---
tags: [software-testing, lecture-4, boundary-value-testing, robust-bvt, worst-case, nextdate, commission-problem]
aliases: [Lecture 4, ST Lecture 4, BVT Examples, Robust BVT, Worst-Case BVT]
lecture: 4
chapter: "Jorgensen Chapter 5"
---

# Lecture 04 — BVT Examples & Robustness

## 📌 Overview

This lecture continues [[Boundary Value Testing]] with deeper coverage of **Robust BVT**, **Worst-Case BVT**, and **Robust Worst-Case BVT**, applied to the [[NextDate Function]] and the [[Commission Problem]]. It also introduces **output boundary value analysis**.

---

## 1 · Robust Boundary Value Testing

### What It Adds

Robust BVT extends normal BVT by adding two extra values per variable:

- **Min−** (below the minimum)
- **Max+** (above the maximum)

### Purpose

> [!definition] Value of Robustness Testing
> The main value of robustness testing is that it **forces attention on exception handling**. It tests how the system behaves when given out-of-range inputs.

### Implementation Philosophy Question

Is it better to:
- Perform **explicit range checking** and use **exception handling** for robust values?
- Or stay with **strong typing**?

The exception handling choice **mandates robustness testing**.

### With Strongly Typed Languages

Robustness testing may be very **awkward** — the language itself may prevent invalid values from being passed.

---

## 2 · Worst-Case Boundary Value Testing

### Motivation

Normal and robust BVT make the **single fault assumption**. Rejecting this means we care about what happens when **more than one variable** has an extreme value.

> [!definition] Worst-Case Analysis
> In electronic circuit analysis, this is called "worst-case analysis"; we use that idea here to generate worst-case test cases.

### How It Works

1. For each variable, take the **five-element set**: `{min, min+, nom, max−, max}`
2. Take the **Cartesian product** of these sets

$$5^n \text{ test cases for } n \text{ variables}$$

### Comparison

| Type | Values per Variable | Test Case Count (n=2) | Test Case Count (n=3) |
|------|-------------------|----------------------|----------------------|
| Normal BVT | {min, min+, nom, max−, max} | $4n + 1 = 9$ | $4n + 1 = 13$ |
| Robust BVT | {min−, min, min+, nom, max−, max, max+} | $6n + 1 = 13$ | $6n + 1 = 19$ |
| **Worst-Case BVT** | {min, min+, nom, max−, max} | $5^n = 25$ | $5^n = 125$ |
| **Robust Worst-Case BVT** | {min−, min, min+, nom, max−, max, max+} | $7^n = 49$ | $7^n = 343$ |

### When to Use Worst-Case

- Physical variables have **numerous interactions**
- **Failure is extremely costly**
- For "really paranoid testing" → **Robust Worst-Case** ($7^n$ test cases)

---

## 3 · The NextDate Function

### Problem Statement

NextDate is a function of **three variables**: month, day, and year. It returns the date of the day after the input date.

**Preconditions:**
- $1 \leq \text{month} \leq 12$
- $1 \leq \text{day} \leq 31$
- $1812 \leq \text{year} \leq 2012$

### Challenge

The NextDate function illustrates the problem of **dependencies in the input domain** — month, day, and year are not independent (e.g., February has fewer days, months have different lengths).

---

## 4 · The Commission Problem

### Problem Statement

A rifle salesperson sells **locks**, **stocks**, and **barrels**:

| Item | Cost | Min Sale | Max Sale |
|------|------|----------|----------|
| Lock | $45 | 1 | 70 |
| Stock | $30 | 1 | 80 |
| Barrel | $25 | 1 | 90 |

### Commission Calculation

| Sales Bracket | Commission Rate |
|---------------|-----------------|
| Up to $1,000 | 10% |
| Next $800 ($1,001–$1,800) | 15% |
| Excess over $1,800 | 20% |

### Sending Telegrams

After each town visit, the salesperson sends a telegram with the count of locks, stocks, and barrels sold. At month-end, a telegram showing `-1` lock sold signals the month is complete.

---

## 5 · Output Boundary Value Analysis

BVT can also be applied to the **output range** of a program, not just the input domain.

**Example (Commission Problem):**
Define test cases based on the **commission brackets** (boundaries at $1,000 and $1,800).

---

## 6 · Practice: CalculateDiscount

| Attribute | Details |
|-----------|---------|
| **Function** | `CalculateDiscount` — applies discount to shopping list |
| **Input** | Total amount of shopping list (IQD) |
| **Output** | Granted discount |

### Discount Rules

| Purchase Amount | Discount |
|-----------------|----------|
| < 50,000 IQD | 0% |
| 50,000 – 99,999.99 IQD | 5% |
| 100,000 – 299,999.99 IQD | 7.5% |
| 300,000 – 499,999.99 IQD | 10% |
| > 500,000 IQD | 12% |

> [!example] Task
> Provide test cases based on **Normal** and **Worst-case** Boundary Value Testing.

---

## 7 · Key Takeaways

1. **Robust BVT** adds Min− and Max+ → tests exception handling
2. **Worst-Case BVT** tests all combinations of extreme values ($5^n$ TCs)
3. **Robust Worst-Case** is the most thorough ($7^n$ TCs) — use when failure is extremely costly
4. The [[NextDate Function]] reveals the problem of **dependent variables** in BVT
5. The [[Commission Problem]] shows how BVT applies to **output ranges** and **commission brackets**
6. BVT can be applied to both **input domains** and **output ranges**

---

## 📚 References

- Jorgensen, P. C. (2014). *Software Testing and Analysis, A Craftsman's Approach*. CRC Press. **Chapter 5.**
- Ammann, P. & Offutt, J. (2008). *Introduction to Software Testing*. Cambridge University Press.
- Myers, G. J. (2012). *The Art of Software Testing*. John Wiley & Sons.
- Pezzè, M. & Young, M. (2008). *Software Testing and Analysis: Process, Principles, and Techniques*. Wiley.

---

← [[Lecture 03 - Boundary Value Testing]] | [[Intro to Software Testing MOC]] | [[Lecture 05 - BVT Limitations and Special Value Testing]] →
