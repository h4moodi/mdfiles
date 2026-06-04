---
tags: [software-testing, lecture-1, introduction, software-failures, verification-validation]
aliases: [Lecture 1, ST Lecture 1, Intro to Testing]
lecture: 1
chapter: "Jorgensen Chapter 1"
---

# Lecture 01 — Introduction to Software Testing

> [!info] Course Info
> **Instructor:** Hossein Hassani · **Department:** Computer Science and Engineering · **Term:** Spring 2026
> Slides adapted from *Jorgensen, P. C. (2014). Software Testing and Analysis, A Craftsman's Approach. CRC Press.*

---

## 1 · Why Software Testing Matters

Software failures are **not rare** — they are costly, dangerous, and ongoing. Testing exists because every piece of software is a potential source of catastrophic failure if its correctness is not verified.

> [!quote] Core Question (Myers, 2012)
> "How do you ensure that all of the software you produce does what it was designed to do and, just as important, **does not do what it isn't supposed to do**?"

---

## 2 · Real-World Software Failures

### Pre-2024 — Historical Catastrophes

The history of software is littered with devastating failures. See curated lists at:
- [Raygun – Costly Software Errors in History](https://raygun.com/blog/costly-software-errors-history/)
- [Therac-25's Deadly Software Tragedy](https://medium.com/@realtestify/the-most-catastrophic-software-bugs-in-history-part-1-therac-25s-deadly-software-tragedy-04b082d12e2c)

### 2024 Failures

| Incident | Impact |
|---|---|
| **CrowdStrike Outage** | Security update caused widespread system failures |
| **Volkswagen Software Crisis** | **$5 billion** loss |
| **Birmingham's Oracle Disaster** | **£38 billion** impact |
| **Concord (Game)** | Gaming's biggest flop — **$200 million** wasted |
| **Jaguar I-Pace Incident** | Self-driving car failed |

### 2025 Failures

| Incident | Date | Cause | Impact |
|---|---|---|---|
| **Marks & Spencer** | April 2025 | Ransomware attack | All online clothing/homeware customers affected for weeks |
| **Optus (Australia)** | Sept 2025 | Firewall upgrade failure | Australians unable to reach emergency services for **13 hours** |
| **Cloudflare** | Nov 18 | Config file error (memory limits) | Thousands of sites (X, ChatGPT, Spotify, Discord, Uber) down for **5h 38min** |
| **Shopify (Cyber Monday)** | Dec 1 | Login authentication failure | 4,000+ merchants; 10%+ US e-commerce; **$15–30M** lost sales; stock fell 5.9% |
| **Cloudflare** | Dec 5 | WAF config change error | 28% of HTTP traffic affected for 25 minutes |

> [!warning] The list goes on!
> These are just highlights. Software failures happen constantly, in every domain.

---

## 3 · The Impossibility of Exhaustive Testing

> [!example] The `Trivial.sum()` Problem (Pezzè & Young, 2008)
> Consider a simple Java method that takes two `int` parameters and returns their sum. How can we exhaustively test it?

**The math:**
- A Java `int` is **32 binary digits**
- Two `int` inputs → $2^{32} \times 2^{32} = 2^{64} \approx 10^{21}$ possible input combinations
- Assume each test takes **1 nanosecond** ($10^{-9}$ sec)
- Total test time ≈ $10^{12}$ seconds ≈ **~30,000 years!**

> [!important] Key Insight
> **Exhaustive testing is impossible** for even the simplest programs. This is the fundamental reason we need *systematic* testing techniques — we must choose our [[Test Case]]s wisely.

---

## 4 · Verification & Validation (V&V) Questions

These are the core questions that drive the discipline of [[Software Testing]] (Pezzè & Young, 2008):

1. **When do [[Verification and Validation]] start? When are they complete?**
2. **What particular techniques** should be applied during development to obtain acceptable quality at an acceptable cost?
3. **How can we assess the readiness** of a product for release?
4. **How can we control the quality** of successive releases?
5. **How can the development process itself be improved** over the course of current and future projects to improve products and make verification more cost-effective?

Additional key questions:
- How much does software testing **cost**?
- Can we **automate** it? To what extent?

---

## 5 · Can AI Do the Testing for Us?

> [!question] The Big Question
> Can AI do the testing for us?

- **If yes:**
  - To what extent?
  - What should we (humans) still know?
  - What is our role?
- **If no:**
  - Could it really be "no"?

This is an open and evolving question that frames the entire module — understanding testing fundamentals is essential *regardless* of AI capabilities.

---

## 6 · Module Overview

The module covers the following areas (refer to the **module descriptor** regularly):

- **Aims** — what the module sets out to achieve
- **Objectives** — specific goals
- **Learning Outcomes** — what you will be able to do
- **Assessments** — how you will be evaluated
- **Delivery Plan** — schedule and pacing
- **References** — required and supplementary reading

> [!tip] Bloom's Taxonomy
> The module aligns with **Bloom's Taxonomy** and the **Anderson-and-Krathwohl Revised Bloom's Taxonomy** for structuring learning outcomes across cognitive levels (Remember → Understand → Apply → Analyze → Evaluate → Create).

---

## 7 · Class Rules

1. **Punctuality:** If you come to class, be on time. Do not ask to enter after the class starts.
2. **No devices:** No electronic devices unless permitted by the lecturer.
3. **No re-entry:** If you walk out, do not come back.
4. **Non-negotiable workload:** Teaching amount, study load, and assignments are fixed.
5. **Exams cover everything:** Everything discussed and taught. **No omissions.**
6. **No postponements:** No extensions for assignments or coursework. Do not ask.
7. **Office hours:** Use them efficiently. You may visit at other times, but the lecturer may be busy.
8. **Communication:** Talk to the lecturer first → email → written note to office → Department Chair.
9. **🎁 Bonus:** Find an error in the course materials → **free coffee** (first person only)!

---

## 8 · Self-Test Exercise

> [!exercise] Calculator Function Testing
> **Specification:**
> - **Name:** `Calculate`
> - **Input:** `String`
> - **Function:** Calculates the string and returns the result. Supports: Addition, Subtraction, Multiplication, Division.
> - **Example:** `Calculate("2+2")` → result: `4`
>
> **Task:** Prepare the inputs to test this function.
>
> Think about: valid operations, edge cases, invalid inputs, division by zero, operator precedence, large numbers, negative numbers, malformed strings…

---

## 9 · Reading & Activities

| Task | Details |
|---|---|
| **Required Reading** | Jorgensen (2014): **Chapter 1** |
| **Supplementary** | Consult references; search online to expand your knowledge |
| **Explore** | UKH library computing section |
| **Next Lecture** | [[Lecture 02 - Basic Concepts and Terminology\|Basic Principles]] |

---

## 10 · References

- **Jorgensen, P. C.** (2014). *Software Testing and Analysis, A Craftsman's Approach.* CRC Press, Taylor & Francis Group.
- **Ammann, P. & Offutt, J.** (2008). *Introduction to Software Testing.* Cambridge University Press.
- **Myers, G. J.** (2012). *The Art of Software Testing.* John Wiley & Sons.
- **Pezzè, M. & Young, M.** (2008). *Software Testing and Analysis: Process, Principles, and Techniques.* John Wiley & Sons.

---
← [[Intro to Software Testing MOC]] | [[Intro to Software Testing MOC]] | [[Lecture 02 - Basic Concepts and Terminology]] →
