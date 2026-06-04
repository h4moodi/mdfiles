---
tags: [software-testing, lecture-10, decision-table, nextdate, cause-effect-graphing, guidelines]
aliases: [Lecture 10, ST Lecture 10, Decision Tables Continued, DT Continued]
lecture: 10
chapter: "Jorgensen Chapter 7"
---

# Lecture 10 — Decision Tables Continued

## 📌 Overview

This lecture applies [[Decision Table Testing]] to the [[NextDate Function]] through **three iterations** of refinement, briefly covers **[[Cause-and-Effect Graphing]]**, and concludes with **guidelines and observations** for effective decision table–based testing.

---

## 1 · Test Cases for the NextDate Function

### Why Decision Tables Work Well for NextDate

The NextDate function illustrates the problem of **dependencies in the input domain** — month, day, and year are not independent. The decision table format lets us emphasize such dependencies by using the notion of the **"impossible" action** → impossible combinations of conditions → impossible rules.

### First Try — 256 Rules

Starting with equivalence classes close to those used in ECT:

**Conditions:**
| Class | Definition |
|-------|------------|
| $M_1$ | Month has **30** days |
| $M_2$ | Month has **31** days |
| $M_3$ | Month is **February** |
| $D_1$ | $1 \leq \text{day} \leq 28$ |
| $D_2$ | $\text{day} = 29$ |
| $D_3$ | $\text{day} = 30$ |
| $D_4$ | $\text{day} = 31$ |
| $Y_1$ | Year is a **leap year** |
| $Y_2$ | Year is **not** a leap year |

**Actions:** a1 = Day invalid for this month, a2 = Cannot happen in a non-leap year, a3 = Compute the next date

This gives $2^8 = 256$ rules — many of which are impossible. The year classes collapse into one condition.

### Second Try — 36 Triples → 16 Rules

Refining with more specific year classes:
- $Y_1$ = Year 2000 (century leap year)
- $Y_2$ = Non-century leap year
- $Y_3$ = Common year

Cartesian product: $3 \times 4 \times 3 = 36$ triples, several impossible. Combining rules with don't care entries → **16 rules**.

**Problems remaining:** December end-of-year and February 28 handling.

### Third Try — 40 Elements → 22 Rules

Further refinement with month classes separating December:

| Class | Definition |
|-------|------------|
| $M_1$ | Month has **30** days |
| $M_2$ | Month has 31 days **(except December)** |
| $M_3$ | Month is **December** |
| $M_4$ | Month is **February** |
| $D_1$ | $1 \leq \text{day} \leq 27$ |
| $D_2$ | $\text{day} = 28$ |
| $D_3$ | $\text{day} = 29$ |
| $D_4$ | $\text{day} = 30$ |
| $D_5$ | $\text{day} = 31$ |
| $Y_1$ | Leap year |
| $Y_2$ | Common year |

Cartesian product: $4 \times 5 \times 2 = 40$ elements. Combining → **22 rules**.

> [!tip] Further Simplification
> Using the algebra of decision tables — if action sets of two rules in an LEDT are identical, we can combine them with a don't care entry. This is the "treated the same" guideline applied to rules.

---

## 2 · Cause-and-Effect Graphing

### Origin

Software community borrowed many ideas from the hardware community. **Cause-and-effect graphing** is a good example — borrowing ideas from digital logic (AND, OR, and NOT gates).

### Basic Operations

| Operation | Symbol | Meaning |
|-----------|--------|---------|
| Identity | `=` | Output equals input |
| AND | `∧` | Output true iff all inputs true |
| OR | `∨` | Output true iff at least one input true |
| NOT | `¬` | Output is inverse of input |
| Mask | — | Input suppresses output |
| Requires | — | One condition requires another |
| Only One | — | Exactly one input must be true |

### Value

The most that can be learned from a cause-and-effect graph is that if there is a problem at an output, the **path(s) back to the inputs** that affected the output can be retraced. There is little support for actually identifying test cases (though it can be mapped to decision tables).

---

## 3 · Guidelines and Observations

### When to Use Decision Table Testing

| Indicator | Description |
|-----------|-------------|
| **a.** | Prominent **if–then–else** logic |
| **b.** | **Logical relationships** among input variables |
| **c.** | Calculations involving **subsets** of input variables |
| **d.** | **Cause-and-effect** relationships between inputs and outputs |
| **e.** | High **cyclomatic complexity** |

### Scaling Up

Decision tables do **not scale up very well** — an LEDT with $n$ conditions has $2^n$ rules.

**Ways to deal with this:**
- Use **extended entry** decision tables
- **Algebraically simplify** tables
- **"Factor"** large tables into smaller ones
- Look for **repeating patterns** of condition entries

### Iteration Helps

As with other techniques, the **first set** of conditions and actions may be unsatisfactory. Use it as a stepping stone and **gradually improve**.

### When DT Is NOT Worth the Trouble

The [[Commission Problem]] is not well served by decision table analysis because very little decisional logic is used. Variables are truly independent, so no impossible rules occur.

---

## 4 · Practice: Car Rental System

| Attribute | Details |
|-----------|---------|
| **System** | Car Rental — checks if customer can rent a vehicle |

### Input Conditions

| Condition | Values |
|-----------|--------|
| **Age** | Under 20, 20–30, Above 30 |
| **Valid Driver's License** | Yes, No |
| **Credit/Debit Card** | Yes, No |
| **Insurance Coverage** | Self, Purchase from rental company |

### Business Rules

- Must have a **valid driver's license**
- Under 20 **cannot rent**
- 20–30 can rent but pay a **"Young Driver Fee"**
- Must have a **credit/debit card** OR pay a **cash deposit**
- Without own insurance → must **purchase from rental company**

### Outputs

| Action | Values |
|--------|--------|
| **Rental Eligibility** | Approved, Rejected |
| **Additional Fee** | None, Young Driver Fee, Cash Deposit Required |
| **Insurance Requirement** | None, Must Purchase Insurance |

> [!example] Task
> Design test cases using the **decision table–based approach**.

---

## 5 · Key Takeaways

1. The [[NextDate Function]] required **three iterations** of decision table refinement
2. Decision tables handle **dependent variables** naturally — impossible rules capture logical impossibilities
3. **Algebraic simplification** of decision tables reduces the number of test cases
4. [[Cause-and-Effect Graphing]] borrows from digital logic but offers limited test case identification support
5. Decision tables work well for **logic-heavy** applications but not for **straight-line computation** (e.g., Commission Problem)
6. Tables don't scale well — use extended entry, factoring, or simplification

---

## 📚 References

- Jorgensen, P. C. (2014). *Software Testing and Analysis, A Craftsman's Approach*. CRC Press. **Chapter 7.**
- Ammann, P. & Offutt, J. (2008). *Introduction to Software Testing*. Cambridge University Press.
- Myers, G. J. (2012). *The Art of Software Testing*. John Wiley & Sons.
- Pezzè, M. & Young, M. (2008). *Software Testing and Analysis: Process, Principles, and Techniques*. Wiley.

---

← [[Lecture 09 - Decision Table Testing]] | [[Intro to Software Testing MOC]] | [[Lecture 11 - Path Testing and DD-Paths]] →
