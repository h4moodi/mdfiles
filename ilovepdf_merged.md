# Introduction to Software Testing

**Department of Computer Science and Engineering**

**Hossein Hassani**

**Spring 2026**

---

## Lecture 1

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 2)*

### Contents

-
Overview
-
About the module
-
Class Rules
-
An Overview of Software Testing and Evaluation
-
A Self Test
-
References

*(Page 3)*

### Software Testing

https://www.cartoonstock.com/directory/s/software_testing.asp?srsltid
=AfmBOor1UtJLI5yevsnGWWQUDRckrYNbPnpFhhMQPen7OIlK4r
xtCVE1

*(Page 4)*

### Software Testing

https://www.cartoonstock.com/search?type=images&keyword=softwar
e+testing&page=1

*(Page 5)*

### Software Testing

Source: http://dilbert.com/ (CANCELED)

*(Page 6)*

### Overview

-
Some Software Failures:
  - Before 2024: so many!
Just see some of the most catastrophic ones at
https://raygun.com/blog/costly-software-errors-history/
https://medium.com/@realtestify/the-most-catastrophic-software-b
ugs-in-history-part-1-therac-25s-deadly-software-tragedy-04b082d
12e2c
And what about after 2024?
-Are we in a better position?

*(Page 7)*

### Overview

-
Some Software Failures:
  -
2024
-CrowdStrike’s outage: Security updates caused issue
-Volkswagen’s Software crisis: $5 billion loss
-Birmingham’s Oracle disaster: £38 billion
-Concord : Gaming’s Biggest Flop: The $200 Million
-The Jaguar I-Pace Incident: Self-Driving car failed
-… and the list goes on!
From https://medium.com/

*(Page 8)*

### Overview

-
Some Software Failures:
  -
2025
-
Marks & Spencer, April 2025, Ransomware attack, All online clothing/homeware
customers, Weeks, cost: ?
-
Optus (Australia), Sept 2025, Firewall upgrade failure, Australian customers
unable to reach emergency services for 13 hours, cost: ?
-
Cloudflare, Nov 18, Configuration file error (memory limits), Thousands of sites
(X, ChatGPT, Spotify, Discord, Uber), 5 hours 38 min, cost:?
-
ShopifyDec 1, 2025,  (Cyber Monday)Login authentication failure4,000+
merchants, 10%+ of US e-commerce, Several hours$15-30M in lost sales; stock
fell 5.9%
-
Cloudflare, Dec 5, Configuration change error (WAF), 28% of HTTP traffic25
minutes, cost: Not disclosed
-
… and the list goes on!
From: Claude.ai

*(Page 9)*

### Overview

-“How do you ensure that all of the software you
produce does what it was designed to do and,
-just as important, does not do what it isn’t
supposed to do?”
(Myers, 2012)

*(Page 10)*

### An Example

-How can we exhaustively test the following
method in Java?
(Pezzè and Young, 2008)

*(Page 11)*

### Self Test

-The Java language definition for the representation of an int:
  - it is 32 binary digits
  - it means 232 × 232 = 264 ≈ 1021 different input to
Trivial.sum() should be tested for the proof of its
correctness.
  - Assume a test takes one ns (10−9 sec)
  - the whole test time ≈ 1012 sec
≈ 30,000 years!

*(Page 12)*

### Overview

-
When do verification and validation start? When are they complete?
-
What particular techniques should be applied during development of
the product to obtain acceptable quality at an acceptable cost?
-
How can we assess the readiness of a product for release?
-
How can we control the quality of successive releases?
-
How can the development process itself be improved over the course
of the current and future projects to improve products and make
verification more cost effective?
(Pezzè and Young, 2008)

*(Page 13)*

### Overview

-
How much software testing costs?
-
Can we automate it?
-
To what extent?

*(Page 14)*

### Big big questions!

-
Can AI do the testing for us?
  - If yes,
-to what extent?
-what should we know?
-what should we do, what is our role?
  - If no,
-could it be no?

*(Page 15)*

### What we do in this module?

-
Aims
-
Objectives
-
Learning Outcomes
-
Assessments
-
Delivery Plan
-
References
Please refer to the module descriptor from time to time !

*(Page 16)*

### Bloom Taxonomy and Anderson-and-Krathwoh-Revised Bloom’s Taxonomy

If you are interested see more:
https://fctl.ucf.edu/teaching-resources/course-design/blooms-taxonomy/#:~:text=Bloom's%20taxonomy%20was%20developed%20to,a%20variety%20of%20cognitive%20levels.
https://www.coloradocollege.edu/other/assessment/how-to-assess-learning/learning-outcomes/blooms-revised-taxonomy.html
https://quincycollege.edu/wp-content/uploads/Anderson-and-Krathwohl_Revised-Blooms-Taxonomy.pdf

*(Page 17)*

### Class Rules

-
If you decide to come to the class, pleas be on time!
-
Please do not ask to enter the class after the class starts (according to the time table).
-
No electronic devices are allowed to be used during the class, unless it is allowed by lecturer.
-
If you walk out the class, pleas do not come back.
-
The amount of teaching, study load, and assignments are not for negotiation.
-
Exams cover everything that has been discussed and taught. No omissions at all.
-
No postponements of due dates for assignments and coursework. Do not think about it, and do not
ask for it, please.
-
Office times are for you; use it efficiently. It is possible to come to my office in other times, but do not
be disappointed if I am busy and couldn't respond to you.
-
Pleas if you have any issues:
  -
Talk to me first,
  -
or drop me an email,
  -
or write me something and drop it to my office.
-
If you did not receive any response, there are other official ways that you can follow, starting from
going to the Department Chair.
-
Finally, if you find errors in the course materials that I give you, you get a free coffee for that (only the
first person who has found it)!

*(Page 18)*

### Self Test

-
Specification of a function:
  -
Name: Calculate
  -
Input: String
  -
Function: Calculates the string and returns back the result. It does the
following arithmetic operations:
-Addition
-Subtraction
-Multiplication
-Division
  -
Example: Calculate (“2+2”) → result: 4
-
Question: Prepare the inputs to test this function.

*(Page 19)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 1.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Basic Principles

*(Page 20)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 21)*

---

## Lecture 2

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 23)*

### Contents

-
Basic concepts
-
Test Case Identification
  -
Specification-based
  -
Code-based
-
Fault Taxonomies
-
Levels of Testing
-
References

*(Page 24)*

### Overview

Some Terminology
-
Error – What people make → mistake.
  - They propagate → if you make an error in interpreting a
requirement, it affects your software all the way!
-
Bug – Mistakes we do during coding.

*(Page 25)*

### Overview

Some Terminology
-
Fault – The result of an error. Defect is another term for this concept.
  - Errors of omission causes:
-Fault →  something is missing that should be present.
  - Example: Not adding a buy transaction to the debit
  - Errors of commission causes:
-Fault → Entering something incorrect into a presentation.
  - Example: Adding a buy transaction to the debit when it is
canceled.

*(Page 26)*

### Overview

Some Terminology
-
Failure – An event that is a result of the execution of a code containing an
error.
-
Incident – Failures might not be easily noticed. An incident is the
symptom associated with a failure that alerts the user that a failure
has occurred.

*(Page 27)*

### Overview

Some Terminology
-
Test – A process to detect the above cases.
  -
The aim:
-find failures
-assure that the software performs correctly
-
Test Case – A scenario and set of inputs and expected outputs that are
related to and tests a software behavior.
  -
TCs must have the followings:
-Precondition
-Input
-Expected output and postconditions
  -
Test cases need to be developed, reviewed, used, managed, and
saved.

*(Page 28)*

### Overview

Some Terminology
-
Test Cases execution:
  - Prepare preconditions
  - Enter the inputs
  - Observing the outputs
  - Comparing these with the expected outputs
  - Ensure that the expected postconditions exist to determine
whether the test passed.

*(Page 29)*

### Specified and implemented program behaviors


*(Page 30)*

### Specified, implemented, and tested behaviors


*(Page 31)*

### Comparing specification-based test case identification methods


*(Page 32)*

### Comparing code-based test case identification methods


*(Page 33)*

### Sources of test cases


*(Page 34)*

### Fault Taxonomies

-
Distinction between process and product:
  - Process refers to how we do something, and
  - Product is the end result of a process.
-
Testing and Software Quality Assurance (SQA) meet when SQA
typically tries to improve the product by improving the process.
-
Testing is clearly more product oriented.
-
SQA is more process oriented.

*(Page 35)*

### Fault Taxonomies

-
Faults can be classified in several ways, based on the:
  - development phase
  - consequences of corresponding failures,
  - difficulty to resolve
  - risk of no resolution
  - etc.

*(Page 36)*

### Fault Taxonomies

-
A reasonable approach could be based on anomaly (fault)
occurrence:
  - One time only
  - Intermittent
  - Recurring
  - Repeatable

*(Page 37)*

### IO Faults

Type
Instances
Input
Correct input not
accepted
Incorrect input accepted
Description wrong or
missing
Parameters wrong or
missing
Output
Wrong format
Wrong result
Correct result at wrong
time (too early, too late)
Incomplete or missing
result
Spurious result
Spelling/grammar
Cosmetic

*(Page 38)*

### Logic Faults

Missing case(s)
Duplicate case(s)
Extreme condition neglected
Misinterpretation
Missing condition
Extraneous condition(s)
Test of wrong variable
Incorrect loop iteration
Wrong operator (e.g., < instead of ≤)

*(Page 39)*

### Computation Faults

Incorrect algorithm
Missing computation
Incorrect operand
Incorrect operation
Parenthesis error
Insufficient precision (round-off, truncation)
Wrong built-in function

*(Page 40)*

### Interface Faults

Incorrect interrupt handling
I/O timing
Call to wrong procedure
Parameter mismatch (type, number)
Incompatible types
Superfluous inclusion

*(Page 41)*

### Data Faults

Incorrect initialization
Incorrect storage/access
Wrong flag/index value
Incorrect packing/unpacking
Wrong variable used
Wrong data reference
Scaling or units error
Incorrect data dimension
Incorrect subscript
Incorrect type
Incorrect data scope
Sensor data out of limits
Off by one
Inconsistent data

*(Page 42)*

### Testing Life Cycle


*(Page 43)*

### Testing Levels (Waterfall Model)


*(Page 44)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 1.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Example scenarios: Chapter 2.

*(Page 45)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 46)*

---

## Lecture 3

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 48)*

### Contents

-
Unit Testing (Boundary Value Testing)
  -
What is Unit?
  -
What is Unit Testing
  -
What is Boundary Value Testing?
  -
The Triangle Problem
  -
References

*(Page 49)*

### What is Unit?

-
Unit is interpreted in different ways.
-
Some interpretations:
  - A single procedure
  - A function
  - A body of code that implements a single function
  - Source code that fits on one page
  - A body of code that represents work done in 4 to 40 hours (as in a
work breakdown structure)
  - The smallest body of code that can be compiled and executed by
itself

*(Page 50)*

### What is Unit?

-
In Object-oriented terminology:
  - The general agreement is that a class is a unit.
  - But,
-methods of a class might be limited by any of the “definitions”
of a unit for procedural code.

*(Page 51)*

### What is Unit?

-
So, finally, what is Unit?
-
When you started developing a software, have a clear definition
among your team about how you define a unit!
-
Meaning:
  - DO NOT TAKE A SINGLE DEFINITION FOR GRANTED!

*(Page 52)*

### Unit as a “Mathematical” Function

-
What is a mathematical function?
  - Informally, a function maps a domain to a range
-
That is what a Unit also does!
Input --------→ function ----------→ output

*(Page 53)*

### Boundary Value Testing

-
Boundary Value Testing or Input Domain Testing
  - A specification-based testing technique.
-
We can also use it to develop range-based test cases.

*(Page 54)*

### Boundary Value Testing

-
Two independent considerations about input domain testing.
  -
Are we concerned with invalid values of variables?
-Normal boundary value testing is concerned only with valid
values of the input variables.
-Robust boundary value testing considers invalid and valid
variable values.
  -
Do we make the “single fault” assumption common to reliability
theory?
-This assumes that faults are due to incorrect values of a single
variable.
-If this is not warranted (i.e., we are concerned with interaction
among two or more variables) we need to take the cross product
of the individual variables.

*(Page 55)*

### Boundary Value Testing

-
Those two considerations give us the following BV testings:
  - Normal boundary value testing
  - Robust boundary value testing
  - Worst-case boundary value testing
  - Robust worst-case boundary value testing

*(Page 56)*

### Triangle Problem

-
Simple version: The triangle program accepts three integers, a, b, and
c, as input(sides of a triangle).
-
These are taken to be sides of a triangle.
-
The output of the program is the type of triangle determined by the
three sides
or NotATriangle.
Equilateral
Isosceles
Scalene

*(Page 57)*

### Triangle Problem


*(Page 58)*

### Triangle Problem


*(Page 59)*

### Boundary Value Testing

Input domain of a function of two variables
F (x1, x2)
a ≤ x1 ≤ b
c ≤ x2 ≤ d

*(Page 60)*

### Boundary Value Testing

Boundary value analysis test cases for a function of two variables
{<x1nom, x2min>, <x1nom, x2min+>, <x1nom, x2nom>, <x1nom, x2max–>, <x1nom, x2max>,
<x1min, x2nom>, <x1min+ , x2nom>, <x1max–, x2nom>, <x1max, x2nom >}

*(Page 61)*

### Generalizing Boundary Value Testing

-
BVT technique is generalized by:
  -
Number of variable
-
Of n variables, hold one at nominal valued and let the others assume min,
min+, nom, max-, max
-
It results as 4n + 1 unique TCs
  -
Types of ranges
-
Depends on the nature of the variables (dates, years, numbers,
alphabets, ...)
-
Discrete with bounded values
  - min, nom, and max values are easy to set
-
No explicit bound
  - Assume bounds (according to expers and app domain)
  -
What about boolean  or logical variables?

*(Page 62)*

### Limitations Boundary Value Testing

-
BV
  -
works well when
-we deal with a function with several independent variables that
represent bounded physical quantities.
-Mathematically, the variables need to be described by a true
ordering relation, in which, for every pair <a, b> of values of
variables, it is possible to say that a ≤ b or b ≤ a.
-For example: temperature, pressure, load
  -
does not work
-Dependent and non-physical variables
-For example: products based on colors, PIN, Tel numbers

*(Page 63)*

### Boundary Value Testing

Normal Boundary Value Test Cases

*(Page 64)*

### Boundary Value Testing

Robustness test cases for a function of two variables

*(Page 65)*

### Boundary Value Testing

Worst-case test cases for a function of two variables

*(Page 66)*

### Boundary Value Testing

(Selected) Worst-Case Boundary Value Test Cases

*(Page 67)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapters 2 and 5.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand your
knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself familiarized with the
resources related to this module.
-
Next Lecture
  -
Unit test (continued)
  -
Software Test and Analysis Framework
  -
Basic Principles

*(Page 68)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 69)*

---

## Lecture 4

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 71)*

### Contents

-
Unit Testing (Boundary Value Testing - continued)
  -
Boundary Value Testing – examples, continued
-
References

*(Page 72)*

### Other terms for boundaries

-
Tools usually refer to the boundary values as:
  - Min
  - Min+
  - Nom (or Mid)
  - Max–
  - Max
-
The robust forms add two values:
  - Min–
  - Max+

*(Page 73)*

### Boundary Value Testing

Robustness test cases for a function of two variables

*(Page 74)*

### Robust Boundary Value Testing

-
The main value of robustness testing is that it forces attention on
exception handling.
-
With strongly typed languages, robustness testing may be very
awkward.
-
This raises an interesting question of implementation philosophy:
  - is it better to perform explicit range checking and use exception
handling to deal with “robust values,” or is it better to stay with
strong typing?
  - The exception handling choice mandates robustness testing.

*(Page 75)*

### Boundary Value Testing

Worst-case test cases for a function of two variables

*(Page 76)*

### Worst-Case Boundary Value Testing

-
Normal and robust boundary value testing make the single fault
assumption of reliability theory.
-
Rejecting single-fault assumption means that we are interested in
what happens when more than one variable has an extreme value.
-
In electronic circuit analysis, this is called “worst-case analysis”; we
use that idea here to generate worst-case test cases.
-
For each variable, we start with the five-element set that contains the
min, min+, nom, max–, and max values.
-
We then take the Cartesian product of these sets to generate test
cases.

*(Page 77)*

### Worst-Case Boundary Value Testing

-
Worst-case boundary value testing is more thorough.
-
That is boundary value analysis test cases are a proper subset of
worst-case test cases.
-
It also represents much more effort:
  - worst-case testing for a function of n variables generates 5n test
cases, as opposed to 4n + 1 test cases for boundary value
analysis.

*(Page 78)*

### Worst-Case Boundary Value Testing

-
Probably the best application for worst-case testing is where
physical variables have numerous interactions, and where failure
of the function is extremely costly.
-
For really paranoid testing, we could go to robust worst-case
testing.
-
This involves the Cartesian product of the seven-element sets we
used in robustness testing resulting in 7n test cases.

*(Page 79)*

### Boundary Value Testing

Robust Worst-case test cases for a function of two variables

*(Page 80)*

### The NextDate Function

-
NextDate is a function of three variables: month, date, and year.
-
It returns the date of the day after the input date.
-
The month, date, and year variables have integer values subject to
these conditions:
  - c1. 1 ≤ month ≤ 12
  - c2. 1 ≤ day ≤ 31
  - c3. 1812 ≤ year ≤ 2012

*(Page 81)*

### Boundary Value Testing

Worst-Case Test Cases

*(Page 82)*

### Boundary Value Testing

Worst-Case Test Cases (continued)

*(Page 83)*

### Boundary Value Testing

Worst-Case Test Cases (continued)

*(Page 84)*

### The Commission Problem

-
A rifle salesperson in the former Arizona Territory sold rifle locks,
stocks, and barrels made by a gunsmith in Missouri.
-
Locks cost $45, stocks cost $30, and barrels cost $25.
-
The salesperson had to sell at least
  - one lock,
  - one stock,
  - and one barrel
  - (but not necessarily one complete rifle) per month
  - production limits were such that the most the salesperson could
sell in a month was 70 locks, 80 stocks, and 90 barrels.

*(Page 85)*

### The Commission Problem

-
After each town visit, the salesperson sent a telegram to the Missouri
gunsmith with the number of locks, stocks, and barrels sold in that
town.
-
At the end of a month, the salesperson sent a very short telegram
showing –1 lock sold.
-
The gunsmith then knew the sales for the month were complete and
computed the salesperson’s commission as follows:
  - 10% on sales up to (and including) $1000,
  - 15% on the next $800,
  - and 20% on any sales in excess of $1800.

*(Page 86)*

### Boundary Value Testing

Worst-Case Test Cases (continued)

*(Page 87)*

### Boundary Value Testing

Output Boundary Value Analysis Test Cases

*(Page 88)*

### Practice

-
CalculateDiscount is a function that calculates a discount that is applied
to a shopping list as follows:
  -
< 50,000 IQD → No discount
  -
>= 50000 and < 100,000 → 5%
  -
>= 100,000 and < 300,000 → 7.5%
  -
>= 300,000 and < 500,000 → 10%
  -
> 500,000 → 12%
-
Input: The total amount of shopping list
-
Output: The granted discount
-
Provide Test Cases to test the mentioned functions based on Normal and
Worst-case Boundary Value Testing.

*(Page 89)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 5.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 90)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 91)*

---

## Lecture 5

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 93)*

### Contents

-
Unit Testing (Boundary Value Testing - continued)
  -
Generalizing boundary value analysis
  -
Limitations of boundary value analysis
  -
Assumptions
  -
Special value testing
-
References

*(Page 94)*

### Generalizing Boundary Value Analysis

-
Two ways:
  - by the number of variables
  - by the kinds of ranges

*(Page 95)*

### Generalizing Boundary Value Analysis

-
The number of variables:
  - For a function of n variables,
-hold all but one at the nominal values
-let the remaining variable assume the min, min+, nom,
max–, and max values
-repeat this for each variable
  - The result is 4n + 1 unique test cases.

*(Page 96)*

### Generalizing Boundary Value Analysis

-
The kind of ranges:
  - Depends on the nature (or more precisely, the type) of the
variables themselves.
  - Depends on programming languages.
  - Regardless, the values for min, min+, nom, max–, and max are
clear from the context.
  - When a variable has discrete, bounded values (e.g.,  variables in
the commission problem, which we saw earlier), the min, min+,
nom, max–, and max are also easily determined.

*(Page 97)*

### Generalizing Boundary Value Analysis

-
The kind of ranges (continued):
  - When no explicit bounds are present, as in the triangle problem,
we usually have to create “artificial” bounds (how?).
  - For other data types, as long as a variable supports an ordering
relation, we can usually infer the min, min+, nominal, max–, and
max values.
-Test values for alphabet characters, for example, would be {a,
b, m, y, and z}.
  - Boundary value analysis does not make much sense for Boolean
variables (Why?)

*(Page 98)*

### Limitations of Boundary Value Analysis

-
Boundary value analysis works well when the program to be tested is
a function of several independent variables that represent bounded
physical quantities.
-
Mathematically, the variables need to be described by a true
ordering relation
  - For every pair <a, b> of values of a variable, it is possible to say
that a ≤ b or b ≤ a
  - Sets of car colors, for example, or football teams, do not support
an ordering relation
  - So, is any form for BVT is appropriate for such variables?

*(Page 99)*

### Limitations of Boundary Value Analysis

-
To repeat, BV analysis test cases are derived from the extrema of:
  - bounded
  - independent variables that refer to physical quantities
  - with no consideration of the nature of the function
  - nor of the semantic meaning of the variables.
-
So, is this method is appropriate for software testing?

*(Page 100)*

### Limitations of Boundary Value Analysis

-
Physical quantity criterion, e.g.,
  - Temperature
  - Pressure
  - Air speed
  - Angle of attack
  - Load
  - ...,
-
Aren’t the boundaries of those attributes crucial?

*(Page 101)*

### Limitations of Boundary Value Analysis

-
Example of logical (vs. physical) variables:
  - PINs
  - mobile numbers
-
What kind of faults you can reveal by testing:
  - PIN values of 0000, 0001, 5000, 9998, and 9999?
  - mobile numbers 000 000 000 and 999 999 999?
  -

*(Page 102)*

### Assumptions

-
Boundary value analysis is based on a critical assumption
  - “single fault” assumption in reliability theory
  - The idea →  failures are only rarely the result of the simultaneous
occurrence of two (or more) faults.

*(Page 103)*

### Assumptions

-
Boundary value analysis is based on a critical assumption
  - “single fault” assumption in reliability theory.
  - The idea →  failures are only rarely the result of the simultaneous
occurrence of two (or more) faults.
-
In software ( particularly software-controlled medical systems) almost
all faults are the result of interaction between a pair of variables.
-
Sometimes more variables are involved.
-
Solution → combinatorial testing (pairwise testing)
  - Will be discussed later.

*(Page 104)*

### Special Value Testing

-
Probably the most widely practiced form of functional testing.
-
Most intuitive and the least uniform.
-
Occurs when to devise a test
  - a tester uses domain knowledge
  - experience with similar programs
  - information about “soft spots” (weak and vulnerable points)

*(Page 105)*

### Special Value Testing

-
You can call special value testing ad hoc testing.
-
No guidelines other than “best engineering judgment.”
-
Very dependent on the abilities of the tester.
-
Regardless of its apparent negatives, can be very useful.

*(Page 106)*

### Special Value Testing

-
Special value testing is highly subjective
-
But  it often results in a more effective set of test cases than the one
BVA can provide (so, software testing is craft!).

*(Page 107)*

### Special Value Testing

-
Despite all the apparent negatives, special value testing can be very useful.
-
If you look carefully at these, especially for the NextDate function, you find
that none is very satisfactory.
-
Special value test cases for NextDate will include several test cases
involving February 28, February 29, and leap years.
-
Are these special? Why?
-
Do I agree that the followings are special values?
Output Special Value Test Cases

*(Page 108)*

### Special Value Testing

-
Despite all the apparent negatives, special value testing can be very
useful.
-
Special value testing is highly subjective
-
But  it often results in a more effective set of test cases than the one
BVA can provide (so, software testing is craft!).
-
Remember the following:
  - a tester uses domain knowledge
  - experience with similar programs
  - information about “soft spots”

*(Page 109)*

### Practice

-
ValidatePasswordConditions is a function that validates whether a chosen
password during sign-up or password change complies with the conditions that
make a password considered highly safe.
-
Input:
  -
passwords
-
Output:
  -
Unacceptable
  -
Weak
  -
Moderate
  -
Safe
  -
Robust
-
Provide Test Case based on Special Value Testing.

*(Page 110)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 5.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 111)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 112)*

---

## Lecture 6

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 114)*

### Contents

-
Unit Testing (Boundary Value Testing - continued)
  -
Random testing
  -
Guidelines for boundary value testing
  -
Tools
-
References

*(Page 115)*

### Random Testing

-
Long history of discussion of random testing.
-
Most of this interest is among academics, and in a statistical sense, it
is interesting.
-
Basic idea:
  - Rather than always choose the min, min+, nom, max–, and max
values of a bounded variable, use a random number generator
to pick test case values.

*(Page 116)*

### Random Testing

-
This avoids any form of bias in testing.
-
It also raises a serious question:
  - how many random test cases are sufficient?
  - We will discuss a proper answer, when we talk about structural
test coverage metrics.

*(Page 117)*

### Random Testing

-
The three examples we discussed so far can get benefit of random
testing.
-
How were the test cases generated?
  - x = Int((b – a + 1) * Rnd + a) was used as the random generator
function for values a ≤ x ≤ b.
  - Int returns the integer part of a floating point number.
  - Rnd generates random numbers in the interval [0, 1].
  - The program keeps generating random test case until at least one
of each output occurs.
  - The program went through seven “cycles” that ended with the
“hard-to-generate” test case.

*(Page 118)*

### Random Testing

Random Test Cases for Triangle Program

*(Page 119)*

### Random Testing

Random Test Cases for Commission Program

*(Page 120)*

### Random Testing

Random Test Cases for NextDate Program

*(Page 121)*

### Guidelines for Boundary Value Testing

-
Test methods based on the input domain of a function (program) are
very basic in the context of all specification-based testing methods,
except for special value testing.
-
A common assumption:  input variables are truly independent.
-
Usually, that is not the case. (can you give some examples?)

*(Page 122)*

### Guidelines for Boundary Value Testing

-
Each of these methods can be applied to the output range of a
program, as we did for the commission problem.
-
Another useful form of output-based test cases is for systems that
generate error messages.
-
The tester should devise test cases to check that error messages are
generated when they are appropriate, and are not falsely generated.

*(Page 123)*

### Guidelines for Boundary Value Testing

-
BVA can also be used for internal variables
  - Loop control variables
  - Indices
  - Pointers
  - ...
-
These are not input variables
-
Bu, errors in the use of these variables are quite common
-
Robustness testing is a good choice for testing internal variables.

*(Page 124)*

### Guidelines for Boundary Value Testing

-
In software testing “the testing pendulum”— is a concept that refers
to the problem of syntactic versus semantic approaches to
developing test cases.
-
Example:
  - Consider a function F of three variables, a, b, and c.
  - The boundaries are
-0 ≤ a < 10,000
-0 ≤ b < 10,000
-0 ≤ c < 18.8.
  -  F = (a – b)/c

*(Page 125)*

### Guidelines for Boundary Value Testing

-
This table shows the normal
BVTCs.
Normal Boundary Value Test Cases for F = (a – b)/c
If we do not consider semantic
knowledge, TCs 1-4 are what a
boundary value testing tool would
generate.
a tool would not generate the
expected output values.
Syntactic version is also problematic.

*(Page 126)*

### Guidelines for Boundary Value Testing

-
Adding the semantic information
  -
F calculates the miles per
gallon of an automobile
  -
a and b are end and start trip
odometer values
  -
c is the gas tank capacity
-
More problems!
1. We must always have a ≥ b.
This will avoid the negative
values of F (test cases 1, 2, 9,
and 10).
2. Test cases 3, 8, and 12–15
all refer to trips of length 0, so
they could be collapsed into
one test case, probably test
case 8.

*(Page 127)*

### Guidelines for Boundary Value Testing

3. Division by zero is an obvious problem, thereby eliminating test case.
Applying the semantic knowledge will result in the better set of case cases in
the following table.
4. The table is still problematic!
-
we never see the effect of boundary values on the tank capacity.
Normal Boundary Value Test Cases for F = (a – b)/c

*(Page 128)*

### Tools

-
Check the followings:
  - ChatGPT, Claude, ...
  - https://www.mobot.io/blog/blackbox-testing-tools-a-complete-guide
  - https://test.io/black-box-testing
  - https://www.ibm.com/products/devops-test/ui
  - https://www.qawolf.com/
  - https://www.ranorex.com/free-trial/
  - https://ldra.com/products/tbextreme/#TBEXT+7
  - https://katalon.com/download
  - ...

*(Page 129)*

### Practice

-
Apply special value testing to the miles per gallon example in the
tables presented on slides 15 and 16.
-
Provide reasons for your chosen test cases.

*(Page 130)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 5.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 131)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 132)*

---

## Lecture 7

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 134)*

### Contents

-
Equivalence Class Testing
  -
Equivalence Classes
  -
Traditional Equivalence Testing
  -
Improved Equivalence Testing
-
References

*(Page 135)*

### Overview

-
How to
  - have a sense of complete testing, and,
  - at the same time, avoiding redundancy in testing?
-
Testing based on equivalence classes addresses those two
concerns.
-
Boundary value testing cannot satisfy those two wishes.
  - Do you remember the tables of test cases? They show massive
redundancy.
  - Look more closely, and you will notice serious gaps.

*(Page 136)*

### Equivalent Classes

-
Why Equivalence Classes are important? (theoretical bases):
  - Partition of a set
-a collection of mutually disjoint subsets
-their union is the entire set
  - Two important implications for testing
-the presence of entire set → a form of completeness of the
test
-the disjointedness →  a form of non-redundancy
-
Example: triangle problem
  - a test case for an equilateral triangle
-(5, 5, 5)
-Can we learn much from test cases (6, 6, 6) and (50, 50, 50)?
https://math24.net/equivalen
ce-classes-partitions.html

*(Page 137)*

### Overview

-
Equivalence class testing is similar to BVT in the following
perspectives:
  - Robustness
  - Single/multiple fault assumption
-
The single versus multiple fault assumption
  - produces the weak/strong distinction
-
The focus on invalid data
  - produces normal versus robust.

*(Page 138)*

### Overview

-
Together they produce the following Equivalence Class testing
  - Weak Normal
  - Strong Normal
  - Weak Robust
  - Strong Robust

*(Page 139)*

### Overview

-
Robust forms have two problems:
  - Oftentimes, the specification does not define what the expected
output for an invalid input should be.
  - Strongly typed languages eliminate the need for the consideration
of invalid inputs.

*(Page 140)*

### Traditional Equivalence Class Testing

-
Based on two values for variables:
  - Valid
  - Invalid
-
Almost identical to weak robust equivalence class testing (will see
later)
-
Focuses on
  - invalid data values (a consequence of the dominant style of
programming in the 1960s and 1970s)
-The validation was an important issue at the time (“Garbage
In, Garbage Out”: GIGO).

*(Page 141)*

### Traditional Equivalence Class Testing

Traditional equivalence class test cases for two variables

*(Page 142)*

### Traditional Equivalence Class Testing

-
The extension to more realistic cases of n variables proceeds as
follows:
1. Test F for valid values of all variables.
2. If step 1 is successful, then test F for invalid values of x1 with
valid values of the remaining variables.
Any failure will be due to a problem with an invalid value of x1.
3. Repeat step 2 for the remaining variables.

*(Page 143)*

### Traditional Equivalence Class Testing

-
Advantage of this process
  - Focuses on finding faults due to invalid data.
-
The kinds of combinations that we saw in the worst-case variations of
boundary value testing were ignored since the GIGO concern was on
invalid data.

*(Page 144)*

### Improved Equivalence Class Testing

-
The key (and the craft!) of equivalence class testing is the choice
of the equivalence relation that determines the classes.
-
Very often, we make this choice by second-guessing the likely
implementation and thinking about the functional manipulations that
must somehow be present in the implementation.
-
We will see this in the following examples.

*(Page 145)*

### Improved Equivalence Class Testing

-
Enriching the function we used in boundary value testing.
-
Function F has two variables, x1 and x2
  - Implementation → A program with input variables as follows:
a ≤ x1 ≤ d, with intervals [a, b), [b, c), [c, d]
e ≤ x2 ≤ g, with intervals [e, f ), [f, g]
[ ] →  closed interval endpoints
( ) → open interval endpoints
These ranges are equivalence classes.

*(Page 146)*

### Improved Equivalence Class Testing

-
The equivalence classes of
valid values are
V1 = {x1: a ≤ x1 < b},
V2 = {x1: b ≤ x1 < c},
V3 = {x1: c ≤ x1 ≤ d}
V4 = {x2: e ≤ x2 < f }
V5 = {x2 : f ≤ x2 ≤ g}
-
Invalid values of x1 and x2
are x1 <a, x1> d, and x2 <e,
x2> g.
-
The equivalence classes of
invalid values are
NV1 = {x1: x1 < a}
NV2 = {x1 : d < x1}
NV3 = {x2: x2 < e}
NV4 = {x2: g < x2}
-
The intervals correspond to some distinction in the program being tested, for
example, the commission ranges in the commission problem.
-
These ranges are equivalence classes.
a ≤ x1 ≤ d, with intervals [a, b), [b, c), [c, d]
e ≤ x2 ≤ g, with intervals [e, f ), [f, g]

*(Page 147)*

### Weak Normal Equivalence Class Testing

-
The equivalence classes V1, V2, V3, V4, V5, NV1, NV2, NV3, and NV4 are disjoint.
-
Their union is the entire plane.
-
Weak normal equivalence class testing:
  -
Use one variable from each equivalence class (interval) in a test case. (Note
the effect of the single fault assumption.)
-
See the following figure for our example (function F).
Weak normal equivalence class test cases

*(Page 148)*

### Strong Normal Equivalence Class Testing

-
Based on the multiple fault assumption
-
We need test cases from each element of the Cartesian product of the equivalence
classes (see the figure. Do you notice the similarity between the pattern of these test cases and the construction of
a truth table in propositional logic?)
-
The Cartesian product guarantees that we have a notion of “completeness”:
  -
we cover all the equivalence classes
  -
we have one of each possible combination of inputs.
Strong normal equivalence class test cases

*(Page 149)*

### Strong Normal Equivalence Class Testing

-
The key to “good” equivalence class testing is
  -
the selection of the equivalence relation.
  -
Watch for the notion of inputs being “treated the same.”
-
Most of the time, equivalence class testing defines classes of the input
domain.
-
Is there any reason for not to define equivalence relations on the output
range of the program function under test?
  -
NO, sometimes that is the simplest approach.
-Think about the the triangle problem.

*(Page 150)*

### Weak Robust Equivalence Class Testing

-
Weak robust?
  -
Robust → consideration of invalid values
  -
Weak → single fault assumption.
-
A simple extension of that for weak normal equivalence class testing—pick
test cases such that each equivalence class is represented.
-
The two additional test cases cover all four classes of invalid values.

*(Page 151)*

### Weak Robust Equivalence Class Testing

-
The process is similar to that for boundary value testing:
1. For valid inputs:
use one value from each valid class (as in what we have called weak
normal equivalence class testing).
2. For invalid inputs:
a test case will have one invalid value and the remaining values will
all be valid. →  a “single failure” should cause the test case to fail.

*(Page 152)*

### Weak Robust Equivalence Class Testing

-
The figure shows the test cases resulting from this strategy.
-
A potential problem with these test cases:
  -
Consider the test cases in the upper left and lower right corners.
  -
Each of the test cases represents values from two invalid equivalence
classes.
  -
Failure of either of these could be due to the interaction of two variables.
Weak robust equivalence class test cases

*(Page 153)*

### Revised Weak Robust Equivalence Class Testing

-
This figure presents a compromise between “pure” weak normal equivalence
class testing and its robust extension.
Revised weak robust equivalence class test cases

*(Page 154)*

### Weak vs. Revised weak robust  Equivalence Class Testing

Revised weak robust equivalence class test cases
Weak robust equivalence class test cases

*(Page 155)*

### Strong Robust Equivalence Class Testing

-
Strong Robust! (redundant?)
  -
Robust
-
consideration of
invalid values
  -
Strong
-
multiple fault
assumption
-
We devise test cases based
on each element of the
Cartesian product of all the
equivalence classes, both
valid and invalid.
Strong robust equivalence class test cases

*(Page 156)*

### Practice

-
Function Name: CalculateShippingCost
  -
Function: Calculates the shipping cost of a package based on its weight,
delivery speed, and destination zone.
  -
Inputs:
-Weight (kg): between 0.1 to 100.0 (inclusive)
-Shipping Speed (string): "standard", "express", "overnight"
-Shipping Area (number): 1 to 10 (inclusive)
  -
Output:
-Amount in IQD
-
Identify valid and invalid equivalence classes
-
Design test cases that cover each class

*(Page 157)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 6.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 158)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 159)*

---

## Lecture 8

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 161)*

### Contents

-
Equivalence Class Testing (ECT) (continued)
  -
Examples
  -
Edge Testing
  -
Guidelines
-
References

*(Page 162)*

### ●

Problem statement mentions four possible outputs can occur: NotATriangle,
Scalene, Isosceles, and Equilateral.
-
We can use these to identify output (range) equivalence classes:
R1 = {<a, b, c>: the triangle with sides a, b, and c is equilateral}
R2 = {<a, b, c>: the triangle with sides a, b, and c is isosceles}
R3 = {<a, b, c>: the triangle with sides a, b, and c is scalene}
R4 = {<a, b, c>: sides a, b, and c do not form a triangle}
Equivalence Class Test Cases for the Triangle Problem

*(Page 163)*

### Equivalence Class Test Cases for the Triangle Problem

-
Four weak normal equivalence class test cases, chosen arbitrarily from
each class are as follows:
No valid subintervals of variables a, b, and c exist
the strong normal TCs are identical to the weak normal ones

*(Page 164)*

### Equivalence Class Test Cases for the Triangle Problem

-
The invalid values for a, b, and c → additional weak robust equivalence class TCs
  -
The invalid values could be
-
Zero
-
any negative number
-
any number greater than 200 (why 200?)

*(Page 165)*

### Equivalence Class Test Cases for the Triangle Problem

-
Here is one “corner” of the cube in three-space of the additional
strong robust equivalence class test cases:

*(Page 166)*

### Equivalence Class Test Cases for the Triangle Problem

-
Notice how thoroughly the expected
outputs describe the invalid input values.
-
Equivalence class testing is clearly
sensitive to the equivalence relation
used to define classes.
-
Here is another instance of craftsmanship.
If we base equivalence classes on the
output domain, we obtain a richer set of
test cases. What are some of the
possibilities for the three integers, a, b, and
c?
-
They can all be equal, exactly one pair can
be equal (this can happen in three ways),
or none can be equal.
D1 = {<a, b, c>: a = b = c}
D2 = {<a, b, c>: a = b, a ≠ c}
D3 = {<a, b, c>: a = c, a ≠ b}
D4 = {<a, b, c>: b = c, a ≠ b}
D5 = {<a, b, c>: a ≠ b, a ≠ c, b ≠ c}
-
As a separate question, we can apply the
triangle property to see if they even
constitute a triangle. (For example, the
triplet <1, 4, 1> has exactly one pair of
equal sides, but these sides do not form a
triangle.)
D6 = {<a, b, c>: a ≥ b + c}
D7 = {<a, b, c>: b ≥ a + c}
D8 = {<a, b, c>: c ≥ a + b}
-
If we wanted to be still more thorough, we
could separate the “greater than or equal
to” into the two distinct cases; thus, the set
D6 would become
D6′ = {<a, b, c>: a = b + c}
D6′′ = {<a, b, c>: a > b + c}
similarly for D7 and D8

*(Page 167)*

### Equivalence Class Test Cases for the NextDate Function

-
NextDate is a function of three variables: month,
day, and year
-
These have intervals of valid values defined as
follows:
M1   = {month: 1 ≤ month ≤ 12}
D1   = {day: 1 ≤ day ≤ 31}
Y1   = {year: 1812 ≤ year ≤ 2012}
-
The invalid equivalence classes are
M2 = {month: month < 1}
M3 = {month: month > 12}
D2 = {day: day < 1}
D3 = {day: day > 31}
Y2 = {year: year < 1812}
Y3 = {year: year > 2012}

*(Page 168)*

### Equivalence Class Test Cases for the NextDate Function

-
A refined version:
  -
Valid classes
M1 = {month: month has 30 days}
M2 = {month: month has 31 days}
M3 = {month: month is February}
D1 = {day: 1 ≤ day ≤ 28}
D2 = {day: day = 29}
D3 = {day: day = 30}
D4 = {day: day = 31}
Y1 = {year: year = 2000}
Y2 = {year: year is a non-century leap year}
Y3 = {year: year is a common year}
Consider two Invalid Classes for each:
(5×6×5) = 150 SR TCs
Strong Normal TCs:
(3×4×3) = 36 SN TCs

*(Page 169)*

### Equivalence Class Test Cases for the NextDate Function

-
These classes yield the following weak normal equivalence class test
cases.
-
As before, the inputs are mechanically selected from the approximate middle
of the corresponding class:

*(Page 170)*

### Equivalence Class Test Cases for the NextDate Function

-
Mechanical selection of input values makes no consideration of our
domain knowledge, thus the two impossible dates.
-
This will always be a problem with “automatic” test case generation,
because all of our domain knowledge is not captured in the choice of
equivalence classes.
-
The strong normal equivalence class test cases for the revised
classes are as follows:

*(Page 171)*

### Equivalence Class Test Cases for the Commission Problem

Valid classes of the input variables
L1 = {locks: 1 ≤ locks ≤ 70}
L2 = {locks = –1} (controls input iteration)
S1 = {stocks: 1 ≤ stocks ≤ 80}
B1 = {barrels: 1 ≤ barrels ≤ 90}
Invalid classes of the input variables:
L3 = {locks: locks = 0 OR locks < –1}
L4 = {locks: locks > 70}
S2 = {stocks: stocks < 1}
S3 = {stocks: stocks > 80}
B2 = {barrels: barrels < 1}
B3 = {barrels: barrels > 90}
-
The input domain is “naturally” partitioned by the limits
on locks, stocks, and barrels.
-
These equivalence classes are exactly those that would
also be identified by traditional equivalence class
testing.
-
The first class is the valid input; the other two are invalid.
-
The input domain equivalence classes lead to very
unsatisfactory sets of test cases.
-
Equivalence classes defined on the output range of the
commission function will be an improvement.
One “corner” of the cube in 3-space of the
additional strong robust equivalence class
test cases
Input space of the commission problem

*(Page 172)*

### Equivalence Class Test Cases for the Commission Problem

Valid classes of the input variables
L1 = {locks: 1 ≤ locks ≤ 70}
L2 = {locks = –1} (controls input iteration)
S1 = {stocks: 1 ≤ stocks ≤ 80}
B1 = {barrels: 1 ≤ barrels ≤ 90}
Invalid classes of the input variables:
L3 = {locks: locks = 0 OR locks < –1}
L4 = {locks: locks > 70}
S2 = {stocks: stocks < 1}
S3 = {stocks: stocks > 80}
B2 = {barrels: barrels < 1}
B3 = {barrels: barrels > 90}

*(Page 173)*

### Equivalence Class Test Cases for the Commission Problem

-
One “corner” of the cube in 3-space of the additional strong
robust equivalence class test cases:
Sales = 45×locks + 30×stocks + 25×barrels
-
We could define equivalence classes of three variables by
commission ranges:
S1 = {<locks, stocks, barrels>: sales ≤ 1000}
S2 = {<locks, stocks, barrels>: 1000 < sales ≤ 1800}
S3 = {<locks, stocks, barrels>: sales > 1800}
-Elements of S1 are points with integer
coordinates in the pyramid near the origin.
-Elements of S2 are points in the “triangular
slice” between the pyramid and the rest of the
input space.
-Elements of S3 are all those points in the
rectangular volume that are not in S1 or in S2.
-All the error cases found by the strong
equivalence classes of the input domain are
outside of the rectangular space in the above
figure

*(Page 174)*

### ●

A hybrid of BVA and ECT
-
When we need it?
  -
When contiguous ranges of a particular
variable forms equivalence classes.
  -
The figure shows three equivalence
classes of valid values for x1 and two
classes for x2.
  -
Assumption:
-
these classes refer to variables
that are “treated the same” in
some application.
  -
There may be faults near the
boundaries of the classes (edge
testing focuses on these potential
faults).
Edge Testing
Normal test values for x1:
{a, a+, b–, b, b+, c–, c, c+, d–, d}
Robust test values for x1 :
{a–, a, a+, b–, b, b+, c–, c, c+, d–, d, d+}
Normal test values for x2:
{e, e+, f–, f, f+, g–, g}
Robust test values for x2 :
{e–, e, e+, f–, f, f+, g–, g, g+}

*(Page 175)*

### ●

One subtle difference:
  -
edge test values do not include the nominal values
-
Once the sets of edge values are determined, edge testing can follow any of
the four forms of equivalence class testing.
-
The numbers of test cases obviously increase as with the variations of
boundary value and equivalence class testing.
Edge Testing

*(Page 176)*

### Guidelines and Observations

1) The weak forms of equivalence class testing (normal or robust) are
not as comprehensive as the corresponding strong forms.
2) If the implementation language is strongly typed (and invalid
values cause run-time errors), no need to use the robust forms.
3) If error conditions are a high priority, the robust forms are
appropriate.
4) Equivalence class testing is strengthened by a hybrid approach
with boundary value testing. (“reuse” the effort made in BVT in
defining the equivalence classes.)

*(Page 177)*

### Guidelines and Observations

5)  Equivalence class testing is indicated when the program function
is complex. In such cases, the complexity of the function can help
identify useful equivalence classes. (remember NextDate function.)
6) Equivalence class testing is appropriate when input data is defined
in terms of intervals and sets of discrete values (system
malfunctions can occur for out-of-limit variable values.)
7) Strong equivalence class testing makes a presumption that the
variables are independent (corresponding multiplication of test
cases raises issues of redundancy). Dependencies often generate
“error” test cases (recall the NextDate function). (Decision table
technique is a solution, which we discuss next week.)

*(Page 178)*

### Guidelines and Observations

8) Several tries may be needed before the “right” equivalence
relation is discovered (recall NextDate example.) When in doubt
(could not find “obvious” or “natural” equivalence relation), try to
second-guess aspects of any reasonable implementation (AKA
“competent programmer hypothesis.”)
9) The difference between the strong and weak forms of equivalence
class testing is helpful in the distinction between progression and
regression testing.

*(Page 179)*

### Practice

-
Inputs:
  -
Weight (kg): between 0.1 to 100.0 (inclusive)
  -
Shipping Speed (string): "standard", "express",
"overnight"
  -
Shipping Area (number): 1 to 10 (inclusive)
-
Output:
  -
Amount in IQD
-
Calculation Rules:
  -
Cost (per kg, in IQD):
-
Standard: 500
-
Express: 1250
-
Overnight: 2500
  -
AreaCoef:
-
Area 1: 1.0
-
Area 2 to 10: Increase 0.10
  -
Final cost = Weight× Cost × AreaCoef
-
Function Name: CalculateShippingCost
  -
Function: Calculates the shipping cost of a package based on its weight, delivery speed, and destination zone.
-
What you should do?
  -
Identify valid and invalid equivalence classes
  -
Design test cases that cover each class
  -
Consider Edge Testing in your test cases design.

*(Page 180)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 5.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 181)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 182)*

---

## Lecture 9

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 184)*

### Contents

-
Decision Table–Based Testing
  -
Decision Tables
  -
Decision Tables Techniques
-
References

*(Page 185)*

### ●

Decision tables are the most rigorous methods for software testing because
of their strong logical basis.
-
Used to represent and analyze complex logical relationships since the early
1960s.
-
Ideal for describing situations in which a number of combinations of actions
are taken under varying sets of conditions.
-
Two closely related methods are used:
  -
cause-and-effect graphing
  -
decision tableau method
  -
These are more difficult to apply and they are not providing much
beyond what decision tables provided, so we only refer to the former at
the end of this topic.
Overview

*(Page 186)*

### ●

Has four portions.
-
We refer to these portions as:
  -
condition stub
  -
condition entries
  -
action stub
  -
action entries
Decision Tables
Portions of a Decision Table
The part to the left of the
bold vertical line is the
stub portion
To the right is the entry
portion.
The part above the
bold horizontal line is
the condition portion
Below is the action
portion

*(Page 187)*

### ●

Rule
  -
A column in the entry
portion
-
Rules indicate which
actions, if any, are taken for
the circumstances indicated
in the condition portion of
the rule.
-
Don’t care (n/a)
  -
the condition is
irrelevant, or
  -
the condition does not
apply
Decision Tables
When c1 and c2 are both
true and c3 is false, then
actions a1 and a3 occur.
when conditions c1, c2,
and c3 are all true,
actions a1 and a2 occur.
Don’t care

*(Page 188)*

### ●

Binary conditions (true/false, yes/no, 0/1)
  -
the condition portion of a decision table is a truth table (from
propositional logic) that has been rotated 90°.
-
This structure guarantees that we consider every possible combination of
condition values.
-
When we use decision tables for test case identification, this completeness
property of a decision table guarantees a form of complete testing.
Decision Tables

*(Page 189)*

### ●

Limited Entry Decision Tables (LETDs)
  -
Decision tables in which all the conditions are binary.
-
Extended Entry Decision Tables (EEDTs)
  -
Conditions are allowed to have several values.
-
Decision tables
-are deliberately declarative (NOT imperative)
  - no particular order is implied by the conditions
  - selected actions do not occur in any particular order
Decision Tables

*(Page 190)*

### ●

How to identify test cases with decision tables?
  -
Take conditions as inputs and actions as outputs.
  -
Conditions might end up referring to equivalence classes of inputs.
  -
Actions refer to major functional processing portions of the item tested.
  -
Take rules as test cases.
Decision Table Techniques
Decision Table for Triangle Problem
-
Decision table can
mechanically be forced to
be complete →
  -
They can provide a
comprehensive set of
test cases.

*(Page 191)*

### ●

Several techniques that produce decision tables are more useful to testers.
  -
A helpful style is to add an action to show when a rule is logically
impossible.
Decision Table Techniques
Decision Table for Triangle Problem
Impossible!

*(Page 192)*

### ●

The choice of conditions can greatly expand the size of a decision table.
Decision Table Techniques
Refined Decision Table for Triangle Problem
(c1: a, b, c form a triangle?) has been expanded to have
more detailed view of the three inequalities of the
triangle property.

*(Page 193)*

### ●When conditions refer to equivalence classes, decision tables

appear in a different way.
Decision Table Techniques
Decision Table with Mutually Exclusive Conditions
mutually exclusive possibilities for the month (conditions for the NextDate problem)
Cannot ever have a rule in which two entries are true.
Here, the don’t care entries (—) mean “must be false.”
Some “experts” use F! to make this point.

*(Page 194)*

### ●

Use of don’t care entries has a
small effect on the way in
which complete decision tables
are recognized.
-
For a limited entry decision
table with n conditions, there
must be 2n independent rules.
-
When don’t care entries really
indicate that the condition is
irrelevant, we can develop a
rule count as follows:
  -
rules in which no don’t
care entries occur count
as one rule
  -
each don’t care entry in a
rule doubles the count of
that rule
Decision Table Techniques
26

*(Page 195)*

### Decision Table Techniques

Applying the method →
wrong results! Why?
Impossible rules.
expand each of the three rules,
replacing the “—” entries with the T
and F possibilities

*(Page 196)*

### Decision Table Techniques

Mutually exclusive conditions
Mutually exclusive conditions
with impossibles
Same as 2.2
Add a missing rule
Same as 3.2
Delete the repetitions → seven rules

*(Page 197)*

### Decision Table Techniques

An Inconsistent Decision Table
What if getting a complete decision table
becomes redundant and/or inconsistent?.
Rule 9 is identical to rule 4.
The action entries are also identical.
But, ifIf the action entries are different,
it a BIG problem!
An Redundant Decision Table
If actions in a redundant rule are
identical to the corresponding part of the
decision table, not a big a problem!

*(Page 198)*

### Decision Table Techniques

-
What if we use this inconsistent
table   to process a transaction
in which c1 is true and both c2
and c3 are false, both rules 4
and 9 apply.
-
Two observations:
1. Rules 4 and 9 are
inconsistent.
2. The decision table is
nondeterministic.
Rules 4 and 9 are inconsistent because
the action sets are different.
The whole table is nondeterministic
because there is no way to decide
whether to apply rule 4 or rule 9.
So what testers should do?
They should care when don’t care entries are used in a decision table.

*(Page 199)*

### Test Cases for the Triangle Problem

-
If we extended the decision table to show both ways to fail an inequality, we
would pick up three more test cases (where one side is exactly the sum of the
other two).
-
Some judgment is required in this because of the exponential growth of rules.
-
In this case, we would end up with many more don’t care entries and more
impossible rules.
Actual values for the possible actions.
Can we do that for impossibles?

*(Page 200)*

### Practice

-
Function: ShoppingDiscount
-
Input:
1. Membership status
-
Regular
-
Premium
2. Purchase amount
-
Above 100,000 IQD
-
Below 100,000 IQD
3. Coupon usage
-
Yes
-
No
-
Output:
  -
Given discount (0%,15%, 20%, 25%)
-
Discount function logic:
  -
Premium members start with a 15% base
discount
  -
Purchases over 100,000 IQD add 20%
discount
  -
Using a coupon adds 5% discount
  -
Regular members with purchases under
100,000 IQD and no coupon get no
discount
  -
The maximum discount is capped at 25%

*(Page 201)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 7.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 202)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 203)*

---

## Lecture 10

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 205)*

### Contents

-
Decision Table–Based Testing (continued)
  -
Example
  -
Cause and Effect Graphing
  -
Guidelines
-
References

*(Page 206)*

### Test Cases for the NextDate Function

-
The NextDate function illustrates the problem of dependencies in the input
domain.
  -
Good example for decision table–based testing
-
Recall that regarding the identification of equivalence classes in it.
-
One of the limitations was that indiscriminate selection of input values from
the equivalence classes resulted in “strange” test cases, such as finding
the next date to June 31, 1812.
-
The problem stems from the presumption that the variables are
independent.

*(Page 207)*

### Test Cases for the NextDate Function

-
If the variable are independent, a Cartesian product of the classes makes
sense.
-
When logical dependencies exist among variables in the input domain,
these dependencies are lost (suppressed) in a Cartesian product.
-
The decision table format lets us emphasize such dependencies:
  -
How?
  -
By using the notion of the “impossible” action
  -
This means impossible combinations of conditions
  -
Which means impossible rules.
-
Let us see how we formulate a decision table of the NextDate function.

*(Page 208)*

### Test Cases for the NextDate Function – First Try

-
The key is: to identify appropriate conditions and actions
-
Suppose we start with a set of equivalence classes close to the one we
had.
M1 = {month: month has 30 days}
M2 = {month: month has 31 days}
M3 = {month: month is February}
D1 = {day: 1 ≤ day ≤ 28}
D2 = {day: day = 29}
D3 = {day: day = 30}
D4 = {day: day = 31}
Y1 = {year: year is a leap year}
Y2 = {year: year is not a leap year}

*(Page 209)*

### Test Cases for the NextDate Function – First Try

-
To highlight impossible combinations
  -
make a limited entry decision table
with the identified conditions and
actions.
-
To show why some rules are impossible,
we might revise our actions. In this case
the changes are:
a1: Day invalid for this month
a2: Cannot happen in a non-leap year
a3: Compute the next date
First Try Decision Table with 256 Rules
This decision table will have 256
(28) rules, many of which will be
impossible.
The equivalence
classes for the
year variable
collapse into one
condition.

*(Page 210)*

### Test Cases for the NextDate Function – Second Try

-
To focus on the leap year, we can use the set of equivalence classes we
identified when we discussed ECT (Equivalence Class Testing).
M1 = {month: month has 30 days}
M2 = {month: month has 31 days}
M3 = {month: month is February}
D1 = {day: 1 ≤ day ≤ 28}
D2 = {day: day = 29}
D3 = {day: day = 30}
D4 = {day: day = 31}
Y1 = {year: year = 2000}
Y2 = {year: year is a non-century leap year}
Y3 = {year: year is a common year}
Here, Y2 is the set of years between 1812 and 2012,
evenly divisible by four excluding the year 2000.
36 triples (Cartesian
product of the ECs), several
of which are impossible

*(Page 211)*

### Test Cases for the NextDate Function – Second Try

`
M1 = {month: month has 30 days}
M2 = {month: month has 31 days}
M3 = {month: month is February}
D1 = {day: 1 ≤ day ≤ 28}
D2 = {day: day = 29}
D3 = {day: day = 30}
D4 = {day: day = 31}
Y1 = {year: year = 2000}
Y2 = {year: year is a non-century leap year}
Y3 = {year: year is a common year}

*(Page 212)*

### Test Cases for the NextDate Function – Second Try

Combining rules with don’t care entries yields
the decision table with 16 rules.

*(Page 213)*

### Test Cases for the NextDate Function – Second Try

Summary of what we did
-
To produce the next date of a
given date, only five possible
actions are needed:
-
incrementing and resetting the day
and month (four cases), and
incrementing the year.
-
We will not let time go backward by
resetting the year.
-
Now, we apply a technique as follows:
  -
Develop an extended entry decision
table
  -
Take a closer look at the action stub
  -
Ensure that the equivalence classes
form a true partition of the input
domain (a partition is a set of disjoint
subsets where the union is the entire
set)
  -
If there were any “overlaps” among
the rule entries,
-
you have a redundant case in
which more than one rule could
be satisfied.

*(Page 214)*

### Test Cases for the NextDate Function – Second Try

Still we have problem!
-
Logically impossible rules helps
to identify the expected outputs
of a test case.
-
When we try to complete the
action entries in this table, we
notice some problems with:
  -
December (in rule 8) and
  -
February 28 in rules 9, 11,
and 12
-
How to fix these? See the third try.
Second Try Decision Table

*(Page 215)*

### Test Cases for the NextDate Function – Third Try

-
We can clear up the end-of-year considerations with a third set of
equivalence classes.
-
This time, we are very specific about days and months, and we revert to
the simpler leap year or non-leap year condition of the first try—so the year
2000 gets no special attention.
M1 = {month: month has 30 days}
M2 = {month: month has 31 days except December}
M3 = {month: month is December}
M4 = {month: month is February}
D1 = {day: 1 ≤ day ≤ 27}
D2 = {day: day = 28}
D3 = {day: day = 29}
D4 = {day: day = 30}
D5 = {day: day = 31}
Y1 = {year: year is a leap year}
Y2 = {year: year is a common year}
Cartesian product →  40 elements.

*(Page 216)*

### Test Cases for the NextDate Function – Third Try

-
Combining rules with don’t care entries →
Table with 22 rules
-
Works better than the previous try.
-
No impossible rules but some redundancy.
  -
Eight of the 10 rules simply increment the
day.
  -
Would we really require eight separate
test cases for this subfunction?
  -
Probably not; but how they can help.
-
The last seven rules focus on February in
common and leap years.
-
Decision tables can help in improving
programming.
-
Their analysis could have been done
during the detailed design.

*(Page 217)*

### Test Cases for the NextDate Function – Third Try

Reduced Decision Table for NextDate Function
We can use the algebra of decision tables to
further simplify these 22 test cases.
If the action sets of two rules in a limited entry
decision table are identical, there must be at least
one condition that allows two rules to be
combined with a don’t care entry.
This is the decision table equivalent of the “treated the same”
guideline that we used to identify equivalence classes.
In a sense, we are identifying equivalence classes of rules.
For example, rules 1, 2, and 3 involve day classes D1, D2,
and D3 for 30-day months.
These can be
combined
similarly for day
classes D1, D2,
D3, and D4 in
the 31-day
month rules, and
D4 and D5 for
February.
(We could do a
fourth try,
showing year
equivalence
classes as in the
second try, but
by now you get
the point.)
Decision Table Test Cases for NextDate

*(Page 218)*

### Test Cases for the Commission Problem

-
The commission problem is not well served by a decision table analysis.
-
This is not surprising because very little decisional logic is used in the
problem.
-
Because the variables in the equivalence classes are truly independent, no
impossible rules will occur in a decision table in which conditions
correspond to the equivalence classes.
-
Thus, we will have the same test cases as we did for equivalence class
testing.

*(Page 219)*

### Cause-and-Effect Graphing

-
Software community borrowed many ideas from the hardware community.
-
Some worked well, some didn’t.
-
Cause-and-effect graphing is a good example of this.
-
Borrowing idea sfrom digital logic (AND, OR, and NOT gates).
Cause-and-effect graphing operations

*(Page 220)*

### Cause-and-Effect Graphing

-
The basic structures can be augmented by less used operations:
  -
Identity
  -
Masks,
  -
Requires
  -
Only One.
-
The most that can be learned from a cause-and-effect graph is that, if there
is a problem at an output, the path(s) back to the inputs that affected the
output can be retraced.
-
There is little support for actually identifying test cases. (I disagree       ,
because it can be mapped to decision tables!)
Cause-and-effect graph for commission problem
Not a good example!

*(Page 221)*

### Guidelines and Observations

-
As with the other testing techniques,
  -
decision table–based testing works well for some applications
-NextDate, for example
  -
is not worth the trouble for others
-Commission problem, for instance (why)?
-
It works well when
  -
a lot of decision making takes place
-the triangle problem), for example
  -
Those in which important logical relationships exist among input
variables
-NextDate, for instance

*(Page 222)*

### Guidelines and Observations

1. The decision table technique is indicated for applications characterized
by any of the following:
a. Prominent if–then–else logic
b. Logical relationships among input variables
c. Calculations involving subsets of the input variables
d. Cause-and-effect relationships between inputs and outputs
e. High cyclomatic complexity (how complex the software under test is)

*(Page 223)*

### Guidelines and Observations

2. Decision tables do not scale up very well
  -
a limited entry table with n conditions has 2n rules.
  -
Ways to deal with this:
-use extended entry decision tables
-algebraically simplify tables
-“factor” large tables into smaller ones
-look for repeating patterns of condition entries

*(Page 224)*

### Guidelines and Observations

3. As with other techniques, iteration helps.
  -
The first set of conditions and actions you identify may be
unsatisfactory.
  -
Use it as a stepping stone and gradually improve on it until you are
satisfied with a decision table.

*(Page 225)*

### Practice

-
Car Rental System
  -
Checks if a customer can rent a vehicle.
-
Input Conditions:
  -
Age
-
Under 20
-
20-30
-
Above 30
-
Valid Driver's License
  -
Yes
  -
No
-
Credit/Debit Card
  -
Yes, No
-
Insurance Coverage
  -
Self
  -
Purchase from rental company
-
How it works:
  -
Customers must have a valid driver's license to rent
  -
Customers under 20 cannot rent vehicles
  -
Customers 20-30 can rent but pay a "Young Driver Fee"
  -
Customers must have either a credit/debit card or pay a
cash deposit
  -
Customers without their own insurance must purchase
insurance from the rental company
-
Actions/Outcomes:
  -
Rental Eligibility
-
Approved
-
Rejected
  -
Additional Fee
-
None
-
Young Driver Fee
-
Cash Deposit Required
  -
Insurance Requirement
-
None
-
Must Purchase Insurance
-
Task:
  -
Design Test Cases for the above scenario based using Decision table-based approach.

*(Page 226)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 7.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 227)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 228)*

---

## Lecture 11

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 230)*

### Contents

-
Path Testing
  -
Program Graphs
  -
Path Testing
-DD-Path (Decision-to-Decision-Path) Testing
-
References

*(Page 231)*

### Overview

-
Code-based testing methods are compliant to
  - rigorous definitions
  - mathematical analysis
  - useful measurement
-
Technology behind path-testing these has been available since the
mid-1970s.
-
Two major techniques, both based on program graph

*(Page 232)*

### Program Graphs

-
Definition
  -
Given a program written in an imperative programming language,
its program graph is a directed graph in which nodes are
statement fragments, and edges represent flow of control.
  -
A complete statement is a “default” statement fragment.
If i and j are nodes in the program
graph, an edge exists from node i to
node j iff  the statement fragment
corresponding to node j can be
executed immediately after the
statement fragment corresponding to
node i.

*(Page 233)*

### Style Choices for Program Graphs

-
Sometimes keep a fragment as a separate node.
-
Sometime it is better to include this with another portion of a statement.
Program graphs of four structured programming constructs
Line numbers refer
to statements and
statement
fragments.

*(Page 234)*

### Statement Fragment

-What is statement fragment?
E.g., line 14 could be split into two lines:
14  Then If (a = b) AND (b = c)
14a Then
14b       If (a = b) AND (b = c)
Source node
Sink node
Sequence
if-then-else
No loop → Acyclic graph
Single entry- Single exit
We exclude nonexecutable
statements such as variable and
type declarations (lines 1-3)
Nested if-
then-else

*(Page 235)*

### Detractors of Path-based Testing

A graph of a simple (but
unstructured!) program; it is
typical of the kind of example
detractors use to show the
(practical) impossibility of
completely testing even
simple programs.
In this program, five paths
lead from node B to node F
in the interior of the loop.
If the loop may have up to
18 repetitions, some 4.77
trillion distinct program
execution paths exist.
(4,768,371,582,030 paths.)
An example of
logical fallacy of
extension!

*(Page 236)*

### DD-Paths

-
Decision-to-decision path (DD-path)
  - The base of the best-known form of code-based testing.
  - A sequence of statements that begins with the “outway” of a
decision statement and ends with the “inway” of the next decision
statement.
  - No internal branches occur in such a sequence.
  - The corresponding code resembles a row of dominoes so that
when the first falls, all the rest in the sequence fall.

*(Page 237)*

### DD-Paths

-
Decision-to-decision path (DD-path)
  - The original DD-path idea was suitable for 2nd gen programming
languages, but not as such for modern ones.
  - For “modern” programming languages, DD-paths are similar to
code “block”s [e.g, a peace of code between {} in Java.]
  - In these languages, the idea works based on the concept of
statement fragment.

*(Page 238)*

### DD-Paths (Segments)

-
We will define DD-paths in terms of paths of
nodes in a program graph.
-
In graph theory, these paths are called chains.
-
Definition
  -
A chain
-
is a path in which the initial and
terminal nodes are distinct, and
-
every interior node has indegree = 1
and outdegree = 1.
  -
Notice that the initial node is 2-connected to
every other node in the chain, and
  -
no instances of 1- or 3-connected nodes
occur.
The length (number of
edges) of the chain in is 6.
Two nodes ni and nj in a directed graph are
0-connected iff no path exists between ni and nj
1-connected iff a semipath but no path exists
between ni and nj
2-connected iff a path exists between ni and nj
3-connected iff a path goes from ni to nj and a
path goes from nj to ni
No other degrees of connectedness exist

*(Page 239)*

### DD-Paths

-
Definition
  -
A DD-path is a sequence of nodes in a program graph such that
Case 1: It consists of a single node with indeg = 0.
Case 2: It consists of a single node with outdeg = 0.
Case 3: It consists of a single node with indeg ≥ 2 or outdeg ≥ 2.
Case 4: It consists of a single node with indeg = 1 and outdeg = 1.
Case 5: It is a maximal chain of length ≥ 1.
Cases 1 and 2 - the unique
source and sink nodes of  as
initial and final DD-paths.
Case 3 -  complex nodes; no
node in more than one DD-path.
Case 4 -  “short branches”;  also
one-fragment, one DD-path.
Case 5 - “normal case,”;  DD-
path is a chain.  “maximal” part
determines the final node of a
normal (nontrivial) chain.

*(Page 240)*

### DD-Path Graph (Control Flow Graph -CFG)

-
Definition
  - Given a program written in an imperative language, its DD-path
graph is the directed graph in which
-nodes are DD-paths of its program graph
-edges represent control flow between successor DD-paths.

*(Page 241)*

### DD-Path Graph

Case 1: It consists of a single node with indeg = 0.
Case 2: It consists of a single node with outdeg = 0.
Case 3: It consists of a single node with indeg ≥ 2 or outdeg ≥ 2.
Case 4: It consists of a single node with indeg = 1 and outdeg = 1.
Case 5: It is a maximal chain of length ≥ 1.
DD-path graph for triangle program
Nodes                 DD-Path             Case of

definition
Node 4 is a case 1 DD-path. Node 23 is a case
2 DD-path.
Nodes 5 through 8 are case 5 DD-paths.
Node 8 is the last node in this DD-path
because it is the last node that preserves the
2-connectedness property of the chain.
Going beyond node 8 to include node 9, we
violate the indegree = outdegree = 1 criterion
of a chain.
If we stop at node 7, we violate the
“maximal” criterion.
Nodes 10, 11, 15, 17, 18, and 21 are case 4
DD-paths.
Nodes 9, 12, 13, 14, 16, 19, 20, and 22 are
case 3 DD-paths. Finally, node 23 is a case 2
DD-path.

*(Page 242)*

### How to Derive a DD-Path Graph?

-
It has a straightforward process
-
You may need some judgment (based on experience!)
-
The last statement in a segment must be
  - a predicate
  - a loop control
  - a break
  - a method exit

*(Page 243)*

### DD-Path Graph

-
Shows which program segments may be followed by others
-
A segment is a node in the DD-Path Graph
-
A conditional transfer of control is a branch represented by an edge
-
An entry node (no inbound edges) represents the entry point to a
method
-
An exit node (no outbound edges) represents an exit point of a
method

*(Page 244)*

### DD-Paths

-
An entry-exit path is a path from the entry node to the exit node
-
Path expressions represent paths as sequences of nodes
-
In practice, it is reasonable to manually create DD-path graphs for
programs up to about 100 source lines.
-
Beyond that, most testers look for a tool.

*(Page 245)*

### Test Coverage Metrics

-
Main reason of DD-paths:
  - they enable very precise descriptions of test coverage.
  - Recall our previous discussions about other methods
-
Test coverage metrics:
  - a device to measure the extent to which a set of test cases covers
(or exercises) a program.
-
Given a program graph, we can define a set of test coverage metrics.
-
We will use them to relate to other published sets of coverage
metrics.

*(Page 246)*

### Node Coverage

-
A set of test cases
  -
when executed
-every node is traversed.
-
Shown as Gnode
-
Nodes correspond to statement fragments →
  -
guarantees that every statement fragment is executed by some test
case.
-
Careful definition of statement fragment nodes →
  -
guarantees that statement fragments that are outcomes of a decision-
making statement are executed.

*(Page 247)*

### Edge Coverage

-
A set of test cases
  - when executed
-every edge in the program graph is traversed.
-
Shown as Gedge
-
The difference between Gnode and Gedge
  - With  Gedge we are certain that all outcomes of a decision-making
statement are executed.

*(Page 248)*

### Chain Coverage

-
A set of test cases
  - when executed
-every chain of length greater than or equal to 2 is
traversed.
-
Shown as Gchain
-
The Gchain coverage is the same as node coverage

*(Page 249)*

### Path Coverage

-
A set of test cases
  -
when executed
-
every path from the source node to the sink node
is traversed.
-
Shown as Gpath
-
It is open to severe limitations when there are loops in a
program.
-
Notice that every loop in a program graph represents a set of
strongly (3-connected) nodes.
-
How to deal with the size implications of loops?
  -
Simply exercise every loop.
  -
Then form the condensation graph of the original program
graph, which must be a directed acyclic graph.

*(Page 250)*

### Miller’s Test Coverage Metrics


*(Page 251)*

### Types of Coverage

Version A
-
Statement Coverage
-
DD-Path Coverage
-
Branch Coverage
-
Simple Loop Coverage
-
Complex Loop Coverage
-
Multiple Condition Coverage
-
“Statistically Significant” Coverage
-
All Possible Paths Coverage
Version B
-
Statement Coverage
-
Decision Coverage
-
Condition Coverage
-
Multiple Decision-Condition Coverage
Version C
-
Chillenski (https://www.faa.gov/sites/faa.gov/files/aircraft/air_cert/design_approvals/air_software/AR-01-18_MCDC.pdf)

*(Page 252)*

### Statement Testing

-
Generally viewed as the bare minimum.
-
If some statements have not been executed by the set of test cases,
  -
there is clearly a severe gap in the test coverage.
-
Our formulation of program graphs allows
  -
statement fragments to be individual nodes →
-C0 metric is covers Gnode.
-
Less adequate than DD-path coverage.
-
Still widely accepted
-
Mandated by ANSI (American National Standards Institute) Standard 187B.

*(Page 253)*

### DD-Path Coverage

-
Traversing DD-path (the C1 metric)
  - each predicate outcome has been executed
-Means traversing every edge in the DD-path graph
C1  ≡ Gchain
-
For if–then and if–then–else statements, this means that both the
true and the false branches are covered (C1p coverage).
-
For CASE statements
  - each clause is covered.

*(Page 254)*

### DD-Path Coverage

-
Beyond this, it is useful to ask how we might test a DD-path.
-
Longer DD-paths generally represent complex computations, which
we can rightly consider as individual functions.
-
For such DD-paths, it may be appropriate to apply a number of
functional tests, especially those for boundary and special values.

*(Page 255)*

### Simple Loop Coverage

-
The C2 metric
  - DD-path coverage (the C1 metric) + loop testing
-
Simple view
  - every loop involves a decision
  - we need to test both outcomes of the decision:
-one is to traverse the loop
-the other is to exit (or not enter) the loop.
-
Equivalent to the Gedge test coverage.

*(Page 256)*

### Simple Loop Coverage (Predicate Outcome Testing)

-
This level of testing requires that every outcome of a decision
(predicate) must be exercised.
-
Because our formulation of program graphs allows statement
fragments to be individual nodes, Miller’s C1p metric is subsumed by
our Gedge metric.

*(Page 257)*

### Simple Loop Coverage (Predicate Outcome Testing)

-
Miller’s test and graph-based coverage do not deal with decisions
made on compound conditions.
-
Identification of dependencies must be made at the code level.
-
This cannot be done just by considering program graphs.
-
The importance of these dependencies is that they are closely related
to the problem of infeasible paths.

*(Page 258)*

### Dependent Pairs of DD-Paths

-We must identify this dependency at the code level.
-We cannot do that just by looking into the program graph.
-Wee look into Cd (C1 + every dependent pair of DD-Paths)
when we talk about data flow testing.

*(Page 259)*

### Dependent Pairs of DD-Paths

-
The most common dependency among pairs of DD-paths is the
define/reference relationship
  - a variable is defined (receives a value) in one DD-path and is
referenced in another DD-path.
-
The importance of these dependencies
  -  they are closely related to the problem of infeasible paths.

*(Page 260)*

### Dependent Pairs of DD-Paths

-
We have good examples of
dependent pairs of DD-paths:
in the up-right figure, C and H
are such a pair, as are DD-
paths D and H.
Nodes                 DD-Path             Case of

definition
The variable IsATriangle is set to TRUE at node C, and
FALSE at node D.
Node H is the branch taken when IsATriangle is TRUE
makes the condition at node F TRUE.
Any path containing nodes D and H is infeasible.
Simple DD-path coverage might not exercise these
dependencies; thus, a deeper class of faults would not
be revealed.

*(Page 261)*

### Complex Loop Coverage

-
Miller’s Cik metric extends the loop coverage metric to include full paths
from source to sink nodes that contain loops.
Concatenated, nested, and knotted loops

*(Page 262)*

### Complex Loop Coverage

-
We can Take a modified boundary value
approach, where the loop index is given its
minimum, nominal, and maximum values.
-
We can push this further to full boundary value
testing and even robustness testing.
-
If the body of a simple loop is a DD-path that
performs a complex calculation, this should also
be tested, as discussed previously.
-
Once a loop has been tested, the tester
condenses it into a single node.
-
If loops are nested, this process is repeated
starting with the innermost loop and working
outward.
Knotted (horrible!)
loops do not appear
if you follow
structured coding,
but appear in
try/catch exception
handling!

*(Page 263)*

### Complex Loop Coverage

-
This results in the same
multiplicity of test cases we
found with boundary value
analysis, which makes
sense, because each loop
index variable acts like an
input variable.
-
If loops are knotted, it will
be necessary to carefully
analyze them in terms of
the data flow methods (will
be discussed in upcoming
lectures).
-
Consider the infinite loop
that could occur if one loop
tampers with the value of
other loop’s index.
1  public class KnottedLoopExample {
2      public static void main(String[] args) {
3          System.out.println("Starting example...");
4
5         int[] numbers = {1, 2, 3, 4, 5};
6          // Outer loop
7          for (int i = 0; i < numbers.length; i++) {
8              System.out.println("Outer loop iteration: " + i);
9              for (int j = 0; j < 2; j++) {
10                  System.out.println("---Inner loop iteration: " + j);
11                   if (j == 1) {
12                      System.out.println("---Resetting outer loop index i to 0");
13                      i = 0;  // Tampers with the outer loop's index!
14                  }
15              }
16              System.out.println("End of outer loop iteration: " + i);
17          }
18          // Could this line be reached?
19          System.out.println("End- KnottedLoopExample");
20      }
21  }

*(Page 264)*

### Multiple Condition Coverage

-
Miller’s CMCC metric addresses
the question of testing decisions
made by compound conditions.
-
Look closely at the compound
conditions in DD-paths B and H.
-
Instead of simply traversing such
predicates to their true and false
outcomes, we should investigate
the different ways that each
outcome can occur.

*(Page 265)*

### Multiple Condition Coverage

-
One possibility is
  - to make a decision table
-a compound condition of three simple conditions will have
eight rules (see the below), yielding eight test cases.

*(Page 266)*

### Multiple Condition Coverage

-
Another possibility is
  - to reprogram compound predicates into nested simple if–
then–else logic, which will result in more DD-paths to cover.
-
An interesting trade off:
  - statement complexity versus path complexity.
-
Importance of multiple condition coverage
  - You cannot neglect/ignore complexity by satisfying the DD-path
coverage.
-
This metric has been refined to Modified Condition Decision
Coverage (MCDC).

*(Page 267)*

### Other Types of Coverage

-
“Statistically Significant” Coverage
  -
The Cstat metric is awkward—what constitutes a statistically
significant set of full program paths?
  -
Maybe this refers to a comfort level on the part of the
customer/user.
-
All Possible Paths Coverage
  -
The subscript in Miller’s C∞ metric says it all—this can be
enormous for programs with loops (see the figure).
  -
This can make sense for programs without loops, and also
for programs for which loop testing reduces the program
graph to its condensation graph.
-
A Closer Look at Compound Conditions
  -
Interested students refer to Section 8.3.3 of Jorgensen
(2014)!

*(Page 268)*

### Practice

-
Draw the Program Graph for the following program segment.
-
Rewrite the program segment such that the compound conditions are replaced by
nested if–then–else statements.
-
Draw the Program Graph for modified program segment.
-
Compare the two graphs and share your observations.
-
Which graph is more complex to check and use for Path-testing?
14  If (a = b) AND (b = c)
15  Then Output (“Equilateral”)
16  Else If (a ≠ b) AND (a ≠ c) AND (b ≠ c)
17              Then Output (“Scalene”)
18              Else Output (“Isosceles”)
19           ndIf
20  EndIf
(Adapted from Exercise 6 - Jorgensen (2014))

*(Page 269)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 8.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Path Testing (continued)

*(Page 270)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 271)*

---

## Lecture 12

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 273)*

### Contents

-
Path Testing (continued)
  -
Basis Path Testing
-
References

*(Page 274)*

### Basis Path Testing

-
Basis has a mathematical notion.
-
Structural testing (code-based testing) can use its attractive possibilities.
-
What is basis?
  -
Certain sets can have a basis.
  -
When they do, the basis has very important properties with respect to
the entire set.

*(Page 275)*

### Basis Path Testing

-
Mathematicians usually define a basis
  -
in terms of a structure called a “vector space,”
-which is a set of elements (called vectors) as well as operations that
correspond to multiplication and addition defined for the vectors.
-
If a half dozen other criteria apply, the structure is said to be a vector space,
and all vector spaces have a basis (in fact they may have several bases).
x
y
z
î = (1,0,0)
ĵ = (0,1,0)
= (0,0,1)
k̂
v = (3,2,1)
3
2
1
Vector Representation
v = 3î + 2ĵ + 1  = (3,2,1)
k̂
3 units in x direction (î)
2 units in y direction (ĵ)
1 unit in z direction ( )
k̂
3D Basis Vectors and Vector Representation
Just as any vector can be represented using basic unit vectors,
any program execution path can be represented using a basis set of independent paths.
This is the core conceptual link between mathematical basis and basis path testing.
AI- generated image by claude.ai

*(Page 276)*

### Basis Path Testing

-A set of basis vectors somehow represents “the essence”
of the full vector space:
  - everything else in the space can be expressed in terms
of the basis, and
  - if one basis element is deleted, this representation
property is lost.

*(Page 277)*

### Basis Path Testing

-
The potential application of this theory for testing
  - if we can view a program as a vector space,
-then the basis for such a space would be a very interesting set
of elements to test.
-
If the basis is okay,
  - we could hope that everything that can be expressed in terms of the
basis is also okay.
-
Thomas McCabe recognized this possibility in the mid-1970s.

*(Page 278)*

### McCabe’s Basis Path Method

-
Below is directed graph that we might take to be the program graph
(or the DD-path graph) of some program.
-
The program does have a single entry (A) and a single exit (G), but
the graph is not based on a structured program, why?

*(Page 279)*

### McCabe’s Basis Path Method

-
McCabe based his view of testing on a major result from graph theory
  -
The cyclomatic number of a strongly connected graph is the number
of linearly independent circuits in the graph.
  -
A circuit is similar to a chain:
-no internal loops or decisions occur
-but the initial node is the terminal node.
  -
A circuit is a set of 3-connected nodes.
Two nodes ni and nj in a directed graph are
0-connected iff no path exists between ni and nj
1-connected iff a semipath but no path exists
between ni and nj
2-connected iff a path exists between ni and nj
3-connected iff a path goes from ni to nj and a
path goes from nj to ni
No other degrees of connectedness exist

*(Page 280)*

### McCabe’s Basis Path Method

-
Strongly connected directed graph
  -
A directed graph having a path/route between every two nodes
-
We can always create a strongly connected graph by:
  -
adding an edge from the (every) sink node to the (every) source node.
-
If the single-entry, single-exit precept is violated,
  -
we greatly increase the cyclomatic number because we need to add
edges from each sink node to each source node.
Making a directed graph
strongly connected

*(Page 281)*

### Cyclomatic Number

-
The cyclomatic number of a (strongly connected)graph
G is
  -
e is the number of edges in G.
  -
n is the number of nodes in G.
  -
p is the number of components in G.
-
V(G) is the number of distinct regions in a strongly
connected directed graph.
-
The set of basis vectors for this space includes V(G)
elements.
V (G)=e−n+ p
`

*(Page 282)*

### Cyclomatic Complexity

-
The cyclomatic number for the following graph
is  V(G) = 5 – 7 + 2 = 0
-
This is not a very good example for
cyclomatic complexity.
-
With strongly connected graphs, the graphs
have larger cyclomatic complexity.

*(Page 283)*

### Cyclomatic Complexity

-
The cyclomatic complexity of the strongly connected graph in the figure is 5; thus,
there are five linearly independent circuits.
-
If we now delete the added edge from node G to node A, these five circuits become
five linearly independent paths from node A to node G.
-
In small graphs, we can visually identify independent paths.
p1: A, B, C, G
p2: A, B, C, B, C, G
p3: A, B, E, F, G
p4: A, D, E, F, G
p5: A, D, F, G
V (G)=e−n+2( p)=10−7+2(1)=5
V (G)=e−n+ p=11−7+1=5
The formula slightly changes for
Not Strongly Connected graphs.
For Strongly Connected graphs.
1
2
3
4
5
6
7
9
10
1
8
11

*(Page 284)*

### Cyclomatic Complexity

Path/Edge Traversal
the edges traversed by each path, and also
the number of times an edge is traversed
1
2
3
4
5
6
7
9
10
1
8

*(Page 285)*

### Observations (Triangle Example)

-
Start with the DD-path graph.
-
E.g.,  a baseline path that corresponds to a
scalene triangle, for example, with sides 3,
4, 5.
-
Flip the decision at node B, we get path p2.
-
Continue the procedure: flip the decision at
node F, get path p3.
-
Continue to flip decision nodes in the
baseline path p1; the next node with
outdegree = 2 is node H.
-
…
-
Notice that we do not have a basis path for
the NotATriangle case.
Basis Paths for Triangle example

*(Page 286)*

### Observations (Triangle Example)


*(Page 287)*

### Essential Complexity

-
Part of McCabe’s work on cyclomatic complexity does more to improve
programming than testing.
-
The basic idea is
  -
to look for the graph of one of the structured programming
constructs,
  -
collapse it into a single node, and
  -
repeat until no more structured programming constructs can be found.

*(Page 288)*

### Essential Complexity

-
McCabe went on to find elemental “unstructures” that violate the precepts of
structured programming.
-
McCabe’s analysis suggests that these violations cannot occur by themselves:
  -
if one occurs in a program, there must be at least one more, so a program
cannot be only slightly unstructured.
-
These cause:
  -
cyclomatic complexity increase →  increase in the minimum number of test cases
-
Next week, we will see that the violations have interesting implications for data flow
testing.

*(Page 289)*

### Unstructures

Violations of structured programming constructs
Structured programming constructs
Each of these violations
contains three distinct
paths, as opposed to the
two paths present in the
corresponding structured
programming constructs;
so one conclusion is that
such violations increase
cyclomatic complexity.

*(Page 290)*

### Condensing

Condensing with respect to structured programming constructs
Try to reduce this graph!

*(Page 291)*

### Unstructures

-
Bottom line for testers:
  -
programs with high cyclomatic complexity require more testing.
-
Of the organizations that use the cyclomatic complexity metric, most set
some guideline for maximum acceptable complexity
  -
V(G) = 10 is a common choice.

*(Page 292)*

### Unstructures

-
What happens if a unit has a higher complexity?
  - Two possibilities:
-simplify the unit or
-plan to do more testing.
-
If the unit is well structured,
  - its essential complexity is 1; so it can be simplified easily.
-
If the unit has an essential complexity greater than 1,
  - often the best choice is to eliminate the violations.

*(Page 293)*

### Guidelines and Observations

-
In specification-based testing, we observed that gaps and redundancies can
both exist and, at the same time, cannot be recognized.
-
The problem was that specification-based testing removes us too far
from the code.
-
The path testing approaches to code-based testing represent the case
where the pendulum has swung too far the other way:
  -
moving from code to directed graph representations and program
path formulations obscures important information that is present in
the code, in particular the distinction between feasible and infeasible
paths.

*(Page 294)*

### Guidelines and Observations

-
No form of code-based testing can reveal missing functionality that is
specified in the requirements.
-
McCabe:  “It is important to understand that these are purely criteria that
measure the quality of testing, and not a procedure to identify test
cases.”
-
He was referring to the DD-path coverage metric and his basis path heuristic
based on cyclomatic complexity metric.
-
Basis path testing therefore gives us a lower boundary on how much
testing is necessary.

*(Page 295)*

### Guidelines and Observations

-
Path-based testing also helps us to find a set of metrics that act as
crosschecks on specification-based testing.
-
We can use these metrics to resolve the gaps and redundancies
question.
-
When we find that the same program path is traversed by several functional
test cases, we suspect that this redundancy is not revealing new faults.
-
When we fail to attain DD-path coverage, we know that there are gaps in the
functional test cases.

*(Page 296)*

### Guidelines and Observations

-
Example:
  -
suppose we have a program that contains extensive error handling,
  -
and we test it with boundary value test cases (min, min+, nom, max–,
and max).
  -
Because these are all permissible values, DD-paths corresponding to
the error-handling code will not be traversed.
-
If we add test cases derived from robustness testing or traditional
equivalence class testing, the DD-path coverage will improve.

*(Page 297)*

### Guidelines and Observations

-
Beyond this rather obvious use of coverage metrics, an opportunity exists for
real testing craftsmanship.
-
Any of the coverage metrics can operate in two ways:
  -
either as a blanket-mandated (comprehensive, without exceptions)
standard (e.g., all units shall be tested to attain full DD-path coverage)
  -
or as a mechanism to selectively test portions of code more
rigorously than others.

*(Page 298)*

### Guidelines and Observations

-
We might choose multiple-condition coverage for modules with complex
logic, while those with extensive iteration might be tested in terms of
the loop coverage techniques.
-
This is probably the best view of structural testing:
  -
use the properties of the source code to identify appropriate
coverage metrics,
  -
then use these as a crosscheck on functional test cases.
  -
When the desired coverage is not attained,
-follow interesting paths to identify additional (special value) test
cases.

*(Page 299)*

### Practice

-
Find basis paths for the following program.
-
Can you use those paths for designing the test case to test the program?
-
Do you need the concepts you learned in specification-based testing in designing the
test cases?
1  function lec12(x, y) {
2      if (x > 0) {
3          if (y > 0) {
4              return x * y;
5          } else {
6              return x + y;
7          }
8      } else {
9          return x / y;
10      }
11  }

*(Page 300)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 5.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Unit Testing continued

*(Page 301)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 302)*

---

## Lecture 13

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 304)*

### Contents

-
Data Flow Testing
  -
Define/Use Testing
  -
Test Coverage Metrics
  -
Slice-based Testing
  -
Program Slicing Tools
-
References

*(Page 305)*

### ●

Has nothing to do with data flow diagrams (DFDs)
-
It is a form of structural testing
-
Focuses on
  -
the points at which variables receive values and
  -
the points at which these values are used (referenced).
-
Data flow testing serves as a “reality check” on path testing
-
Many of the data flow testing proponents (and researchers) see this approach as a
form of path testing.
-
Data flow and slice-based testing are cumbersome at the unit level
-
But they are well suited for object-oriented code.
Overview

*(Page 306)*

### ●

Two mainline forms of data flow testing:
1-  a set of basic definitions and a unifying structure of test coverage
metrics
2- based on a concept called a “program slice”
-
Both formalize intuitive behaviors of testers.
-
Both start with a program graph, both move back in the direction of functional
testing.
-
Both are difficult to perform manually
-
Few commercial tools exist to support them
-
Both are helpful for coding and debugging
Overview

*(Page 307)*

### ●

Most programs deliver functionality in terms of data.
-
Variables that represent data somehow receive values.
-
These values are used to compute values for other variables.
Overview
What IDEs Can Do Now?
Early data flow analyses often centered on a set of faults that are now
known as define/reference anomalies:
- A variable that is defined but never used (referenced)
- A variable that is used before it is defined
- A variable that is defined twice before it is used
Each of these anomalies can be recognized from the concordance of a
program.
Because the concordance information is compiler generated, these
anomalies can be discovered by what is known as static analysis:
finding faults in source code without executing it.

*(Page 308)*

### ●

Assumption:
  -
Having a program graph, G(P) – (the program has set of variables V)
  -
Following the structured programming precepts (rules)
Define/Use (defuse) Testing
G(P) Properties
Has a single-entry node and a single-exit node
Edges from a node to itself is not allowed
Paths, subpaths, and cycles -  same as defined before
PATHS(P) represents the set of all paths in P

*(Page 309)*

### ●

Defining node - DEF(v, n)
  -
Node n

∈G(P)
  -
Variable v

∈V
  -
Iff the value of variable v is
defined as the statement
fragment corresponding to
node n.
[Where a variable assigned
a value]
Definitions
-
Usage node - USE(v, n)
  -
Node n

∈G(P)
  -
Variable v

∈V
  -
Iff the value of the variable v is
used as the statement
fragment corresponding to
node n.
[Where a variable’s value is
accessed]

*(Page 310)*

### DEF-USE Example


*(Page 311)*

### ●

Predicate use – P-use
Iff the n is a predicate
Otherwise, it is a computation use
(C-use)
Predicate → always outdegree ≥ 2
C-use → always outdegree ≤ 1
Definitions
-
Definition/use path - du-path
a path in PATHS(P)
(DEF(v, m) and USE(v, n))
{v

∈V, m: initial node, n:
final node of the path}
∃
-
Definition-clear path - dc-path
a definition/use path in PATHS(P)
(DEF(v, m) and USE(v, n))

{v

∈V, m: initial node,
n: final node of the path,
k
dc-path in which
∈
k defines v}
∄

*(Page 312)*

### Definitions - Example


*(Page 313)*

### ●

Testers should notice how these definitions capture the essence of
computing with stored data values.
-
Du-paths and dc-paths describe the flow of data across source
statements from points at which the values are defined to points at
which the values are used.
-
Du-paths that are not definition clear are potential trouble spots.
-
Using du-paths you can:
  -
identify points for variable “watches” and breakpoints in an IDE.
Define/Use (defuse) Testing

*(Page 314)*

### Example

Commission problem and its program graph

*(Page 315)*

### Example

DD-path graph of commission problem pseudocode.

*(Page 316)*

### Example

Du-paths for locks
DD-paths

*(Page 317)*

### Example

Define/Use Nodes for Variables in Commission Problem
Selected Define/Use Paths

*(Page 318)*

### Example

Define/Use Paths for Commission

*(Page 319)*

### ●

We analyzing a program with definition/use paths to define a set of test
coverage metrics.
  -
known as the Rapps–Weyuker data flow metrics.
-
The first three of these are equivalent to three of Miller’s metrics (recall path
testing lectures)
  -
All-Paths, All-Edges, and All-Nodes
-
The others presume that define and usage nodes have been identified for all
program variables, and that du-paths have been identified with respect to
each variable.
Test Coverage Metrics

*(Page 320)*

### ●

In the following definitions:
  -
T is a set of paths in the program graph G(P) of a program P, with the
set V of variables.
-
It is not enough to take the cross product of the set of DEF nodes with
the set of USE nodes for a variable to define du-paths.
-
This mechanical approach can result in infeasible paths.
-
We assume that the define/use paths are all feasible.
Test Coverage Metrics

*(Page 321)*

### Test Coverage Metrics - Definitions

-
All-Defs
  -
iff for every variable v

∈V, T
contains definition-clear paths from
every defining node of v to a use of
v.
-
All-Uses
  -
iff for every variable v

∈V, T
contains definition-clear paths from
every defining node of v to every
use of v, and to the successor node
of each USE(v, n).
-
All-P-Uses/Some C-Uses
  -
iff for every variable v

∈V, T
contains definition-clear paths from
every defining node of v to every
predicate use of v; and if a
definition of v has no P-uses, a
definition-clear path leads to at
least one computation use.
-
All-C-Uses/Some P-Uses
  -
iff for every variable v

∈V, T
contains definition clear paths from
every defining node of v to every
computation use of v; and if a
definition of v has no C-uses, a
definition-clear path leads to at
least one predicate use.
-
All-DU-paths
  -
Iff for every variable v

∈V, T
contains definition-clear paths from
every defining node of v to every
use of v and to the successor node
of each USE(v, n), and that these
paths are either single loop
traversals or they are cycle free.

*(Page 322)*

### ●

Define/use testing provides a rigorous, systematic way to examine points at
which faults may occur.
Hierarchy of Data Flow Coverage Metrics
Rapps–Weyuker hierarchy of data flow coverage metrics

*(Page 323)*

### ●

Program slices concept goes back to the early 1980s.
-
Took about 20 years to move a seminal idea into industrial practice.
-
Informally, a program slice is
  -
a set of program statements that contributes to, or affects the value
of, a variable at some point in a program.
-
This notion of slice corresponds to other disciplines as well.
  -
Compare the idea with other with the way we study other disciplines.
Slice-Based Testing

*(Page 324)*

### ●

Program slicing is not a viable manual
approach.
-
While having its place, the actual learning
benefit is not substantial
-
Most of slicing tools are either academic or
experimental.
-
Few commercial tools exist.
-
The more elaborate tools feature
interprocedural slicing, something clearly useful
for large systems.
-
Much of the market uses program slicing to
improve the program comprehension that
maintenance programmers need.
-
JSlice, will be appropriate for object-oriented
software.
Program Slicing Tools
Selected Program Slicing Tools

*(Page 325)*

### ●

Consider the following function:
  -
List Defs
  -
List Uses
  -
List Du-paths
  -
Devise test case based on Du-paths
Practice
1  CalcNetAmount(double purchaseAmnt, int cutsomerType, int loyaltyYears){
2      double discount = 0;
3
4      if (purchaseAmnt > 100) {
5          discount = 0.05; }
6
7      if (cutsomerType == 1) {
8          discount += 0.05 ; }
9
10          if (loyaltyYears > 5) {
11              discount += 0.05;}
12
13      return (purchaseAmnt * (1 - discount));
14  }

*(Page 326)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 9.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Integration testing

*(Page 327)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 328)*

---

## Lecture 14

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 330)*

### Contents

-
Integration Testing
  -
Decomposition-Based Integration
-Top–Down Integration
-Bottom-up Integration
-Sandwich Integration
-
References

*(Page 331)*

### ●

September 1999
  -
the Mars Climate Orbiter mission failed
  -
Before failing, it successfully traveling 416 million miles in 41 weeks.
  -
It disappeared just as it was to begin orbiting Mars.
-
The fault should have been revealed by integration testing:
  -
Lockheed Martin Astronautics used acceleration data in English units
(pounds), while the Jet Propulsion Laboratory did its calculations with
metric units (newtons).
-
NASA announced a $50,000 project to discover how this could have
happened.
-
You will find out this “how” in this lecture.
Overview

*(Page 332)*

### ●

Of the three distinct levels of software testing—unit, integration, and system
integration testing is the least well understood of these.
-
Therefore, in practice, it is the phase most poorly done.
Overview
How Craftspersons Are Recognized?
They two essential characteristics:
- A deep knowledge of the tools of their trade
- A similar knowledge of the medium in which they work
So they understand their tools in terms of how they work with the medium.

*(Page 333)*

### ●

Mainline introductory software engineering texts typically present four
integration strategies based on the functional decomposition tree of the
procedural software:
  -
Top–down
  -
Bottom–up
  -
Sandwich
  -
“big bang”
Decomposition-Based Integration

*(Page 334)*

### ●

Top–down, Bottom–up, and Sandwich describe the integration order in
which units are to be integrated.
-
Big bang works differently.
  -
all the units are compiled together and tested at once.
  -
The drawback to this is that when (not if!) a failure is observed, few
clues are available to help isolate the location(s) of the fault. (Recall the
distinction between faults and failures.)
Decomposition-Based Integration

*(Page 335)*

### ●

The functional decomposition tree is the basis for integration testing
  -
it is the main representation, usually derived from final source code
  -
shows the structural relationship of the system with respect to its units
-
All these integration orders presume that
  -
the units have been separately tested
-
The goal of decomposition-based integration is
  -
to test the interfaces among separately tested units
Decomposition-Based Integration

*(Page 336)*

### ●

A functional decomposition tree reflects the lexicological inclusion of
units,
  -
The inclusion is in the order in which they need to be compiled
  -
This is to assure the correct referential scope of variables and unit
names.
-
Our familiar NextDate unit is extended to a main program, Calendar, with
procedures and functions (see next slide).
Decomposition-Based Integration

*(Page 337)*

### Decomposition-Based Integration – Example (Calendar)

1  Main Calendar
2  Data Declarations
3  mm, dd, yyyy, dayNumber, dayName, zodiacSign
4  Function isLeap (input yyyy, returns T/F)
5
(isLeap is self-contained)
6
End Function isLeap
7  Procedure getDate (returns mm, dd, yyyy, dayNumber)
8
Function isValidDate (inputs mm, dd, yyyy; returns T/F)
9
Function lastDayOfMonth (inputs mm, yyyy, returns 28, 29, 30, or 31)
10
lastDayOfMonth body
11
(uses isLeap)
12
end lastDayOfMonth body
13
End Function lastDayOfMonth
14
isValidDate body
15
(uses lastDayOfMonth)
16
end isValidDate body
17
End Function isValidDate
18
Procedure getDigits(returns mm, dd, yyyy)
19
(uses Function isValidDate)
20
End Procedure getDigits
21  Procedure memorialDay (inputs mm, dd, yyyy; returns yyyy)
22
Function isMonday (inputs mm, dd, yyyy; returns T/F)
23
(uses weekDay)
24
End Function isMonday
25
memorialDaybody
26
isMonday
27
end memorialDay
28  End Procedure memorialDay
29  Procedure friday13th (inputs mm, dd, yyyy; returns mm1, dd1, yyyy1)
30
Function isFriday (inputs mm, dd, yyyy; returns T/F)
31
(uses weekDay)
32
End Function isFriday
33
friday13th body
34
(uses isFriday)
35
end friday13th
36  End Procedure friday13th
37  getDate body
38
getDigits
39
isValidDate
40
dateToDayNumber
41  end getDate body
42  End Procedure getDate
43  Procedure nextDate (input daynum, output mm1, dd1, yyyy1)
44
Procedure dayNumToDate
45
dayNumToDate body
46
(uses isLeap)
47
end dayNumToDate body
48  nextDate body
49
dayNumToDate
50  end nextDate body
51  End Procedure nextDate
52  Procedure weekDay (input mm, dd, yyyy; output dayName)
53
(uses Zeller’s Congruence)
54  End Procedure weekDay
55  Procedure zodiac (input dayNumber; output dayName)
56
(uses dayNumbers of zodiac cusp dates)
57  End Procedure zodiac
58  Main program body
59
getDate
60
nextDate
61
weekDay
62
zodiac
63
memorialDay
64
friday13th
65  End Main program body
1  Main  Calendar
2  Function isLeap
3  Procedure weekDay
4  Procedure getDate
5
Function isValidDate
6
Function lastDayOfMonth
7
Procedure getDigits
8  Procedure memorialDay
9
Function isMonday
10  Procedure friday13th
11
Function isFriday
12  Procedure nextDate
13
Procedure dayNumToDate
14  Procedure zodiac

*(Page 338)*

### ●

The figure shows a condensed “skeleton” as the basis for the functional
decomposition according to Calendar program (previous slide).
Functional decomposition tree for the Calendar program
Functional decomposition of Calendar program

*(Page 339)*

### ●

Root of the tree
  -
Main program
-
Stub
  -
Any lower-level unit that is called by the main program.
  -
Pieces of throwaway code that emulate a called unit.
  -
The tester hard codes to respond correctly to the request from the calling/invoking
unit
  -
The goal of the first step is to check that the main program functionality is correct.
  -
Once the main program has been tested, we replace one stub at a time, leaving the
others as stubs.
Top–Down Integration
First step in top–down integration
Stub for zodiac: Main calls zodiac with 05, 27,
2012, zodiacStub would return “Gemini.”
In extreme practice, the response might be
“pretend zodiac returned Gemini.”

*(Page 340)*

### ●

The stub replacement process proceeds in a breadth-first traversal of the
decomposition tree until all the stubs have been replaced.
-
The “theory” of top–down integration is:
  -
as stubs are replaced one at a time, if there is a problem, it must be
with the interface to the most recently replaced stub.
Top–Down Integration

*(Page 341)*

### ●

The problem is that a functional decomposition is deceptive.
-
Because it is derived from the lexicological inclusion required by most
compilers, the process generates impossible interfaces.
Top–Down Integration
Calendar main never
directly refers to either
isLeap or weekDay, so
those test sessions could not
occur.

*(Page 342)*

### Top–Down Integration

Next three steps in top–down integration
gray-shaded units are all
stubs. The goal of the first
step is to check that the
main program functionality
is correct

*(Page 343)*

### ●

Bottom–up integration is a “mirror image” to the top–down order.
-
The difference that stubs are replaced by driver modules
-
Driver
  -
Emulate units at the next level up in the tree.
Bottom–Up Integration

*(Page 344)*

### Bottom–Up Integration

First steps in bottom–up integration
Bottom–up integration for zodiac
gray-shaded units are drivers
In this case, the Calendar driver would
probably call zodiac with 36 test dates
that are the day before a cusp date, the
cusp date, and the day after the cusp date.
The cusp date for Gemini is May 21, so
the driver would call zodiac three times,
with May 20, May 21, and May 22.
The expected responses would be
“Taurus,” “Gemini,” and “Gemini,”
respectively.

*(Page 345)*

### ●

Bottom–up integration begins with the leaves of the decomposition tree,
-
Use a driver version of the unit that would normally call it to provide it with
test cases.
-
Note the similarity to test driver units at the unit level.
-
As units are tested, the drivers are gradually replaced, until the full
decomposition tree has been traversed.
-
Less throwaway code exists in bottom–up integration, but the problem
of impossible interfaces persists.
Bottom–Up Integration

*(Page 346)*

### ●

Sandwich integration is a combination of top–down and bottom–up
integration.
-
If we think about it in terms of the decomposition tree, we are really only
doing big bang integration on a subtree .
Sandwich Integration

*(Page 347)*

### ●

Less stub and driver development effort
-
Will be offset to some extent by the added difficulty of fault isolation that
is a consequence of big bang integration.
-
The size of a sandwich could be as small as dainty finger sandwiches or as
large as Dagwood-style sandwiches!
Sandwich Integration
https://www.unileverfoodsolutions.com.au/recipe/citrus-po
ached-chicken-finger-sandwiches-R0081891.html

https://en.wikipedia.org/wiki/Dag
wood_sandwich

*(Page 348)*

### ●

A sandwich is
  - a full path from the root to leaves of the functional decomposition
tree.
-
Also note that the fault isolation capability of the top–down and
bottom–up approaches is sacrificed.
-
No stubs nor drivers are needed in sandwich integration.
Sandwich Integration
In the figure, the set of
units is almost
semantically coherent,
except that isLeap is
missing.
This set of units could be
meaningfully integrated,
but test cases at the end of
February would not be
covered.

*(Page 349)*

### ●

With the exception of big bang integration, the decomposition-based
approaches are all intuitively clear.
  - Build with tested components.
  - See a failure → suspect the most recently added unit
-
Integration testing progress is easily tracked against the
decomposition tree.
Pros and Cons

*(Page 350)*

### ●

If the tree is small
  -
it is a nice touch to shade in nodes as they are successfully integrated.
-
The top–down and bottom–up terms suggest
  -
breadth-first traversals of the decomposition tree,
  -
but this is not mandatory.
  -
You could use full-height sandwiches to test the tree in a depth-first
manner.
Pros and Cons

*(Page 351)*

### ●

One of the most frequent objections to functional decomposition and
waterfall development is that
  -
both are artificial
  -
both serve the needs of project management more than the needs of
software developers
-
This holds true also for decomposition-based testing.
-
The whole mechanism is that units are integrated with respect to structure;
this presumes that correct behavior follows from individually correct units
and correct interfaces. (Practitioners know better.)
-
Another drawback
  -
the development effort for stubs or drivers
  -
this is compounded by the retesting effort.
Pros and Cons

*(Page 352)*

### ●

You have your team for the semester assignment, don’t you?
-
You selected a system and it is ready for testing, isn’t it?
-
Assuming the answers to the two questions above are positive, you can plan
and practice on the Integration Testing, can’t you?
Practice

*(Page 353)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 13.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Integration Testing (continued)

*(Page 354)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 355)*

---

## Lecture 15

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 357)*

### Contents

-
Integration Testing
  -
Call Graph–Based Integration
  -
Recommendations
-
References

*(Page 358)*

### ●

A drawback of decomposition-based integration:
  -
the basis is the functional decomposition tree.
  -
This leads to impossible test pairs.
-
To resolve this deficiency, we use the call graph
Call Graph–Based Integration
Call graph of Calendar program
The call graph is developed by
considering units to be nodes.
If unit A calls (or uses) unit B,
there is an edge from node A
to node B.

*(Page 359)*

### ●

Edges in the call graph refer to actual execution–time connections.
-
That helps to avoid all the problems we saw in the decomposition tree–
based versions of integration.
-
Stubs and drivers are as before.
-
This will work well, and it preserves the fault isolation feature of the
decomposition-based approaches.
Call Graph–Based Integration

*(Page 360)*

### ●

The stubs could operate as follows:
  -
When the Calendar main program calls getDateStub, the stub might return a
correct date (e.g., May 27, 2013).
  -
The zodiacStub would return “Gemini,” and so on.
  -
Once the main program logic is tested, the stubs would be replaced with
actual code.
  -
It will all work well when stubs and drivers are based on the call graph
rather than the functional decomposition.
Call Graph–Based Integration - Example
Call graph–based top–down integration of Calendar program

*(Page 361)*

### ●

Now we can enjoy (!) (don’t you agree?       ) what we learned in using
graph theory.
-
Call graph is a directed graph
  -
so, why not use it the way we used program graphs?
-
This leads us to two new approaches to integration testing:
  -
pairwise integration
  -
neighborhood integration
Call Graph–Based Integration

*(Page 362)*

### ●

The idea is to eliminate the stub/driver development effort.
-
Why not use the actual code? Isn’t it similar to big bang integration?
-
No, because we restrict a session to only a pair of units in the call graph.
-
The end result is that we have one integration test session for each edge in
the call graph.
-
Pairwise integration results in an increased number of integration sessions when
a node (unit) is used by two or more other units.
Pairwise Integration
Three pairs for pairwise integration

*(Page 363)*

### ●

The Calendar example:
  -
top–down integration:
-15 separate sessions (one for each stub replacement);
  -
pairwise integration
-19 sessions (one for each edge in the call graph).
-
So what do we save?
  -
A reduction in stub/driver development.
Pairwise Integration - Example
Pairwise integration
(gray nodes)

*(Page 364)*

### ●

Main advantage
  -
The high degree of fault isolation.
  -
If a test fails, the fault must be in one of the two units.
-
Biggest drawback
  -
For units involved on several pairs, a fix that works in one pair may not
work in another pair.
Pairwise Integration
Three pairs for pairwise integration

*(Page 365)*

### ●

Mathematics can carry us still further by borrowing the notion of a
neighborhood from topology (graph theory is a branch of topology.)
-
Neighborhood of a node
  -
Is the set of nodes that are one edge away from the given node.
  -
Technically, this is a neighborhood of radius 1.
  -
In larger systems, it makes sense to increase the neighborhood radius.
Neighborhood Integration

*(Page 366)*

### Neighborhood Integration

Neighborhoods of Radius 1 in Calendar Call Graph
Calendar call graph with units replaced by numbers

*(Page 367)*

### Neighborhood Integration

Adjacency Matrix of Calendar Call Graph
How to compute the number of neighborhoods
for a given call graph?
Each interior node will have one
neighborhood, plus one extra in case leaf nodes
are connected directly to the root node.
Interior node :
a nonzero indegree & nonzero outdegree.
The column sums show the
indegrees of each node, and the
row sums show the outdegrees.
Interior nodes = nodes - (source nodes + sink nodes)
Neighborhoods = interior nodes + source nodes
Neighborhoods = nodes – sink nodes

*(Page 368)*

### ●

The call graph–based integration techniques move away from a purely
structural basis toward a behavioral basis.
-
The underlying assumption is an improvement.
-
The neighborhood-based techniques also reduce the stub/driver
development effort.
-
Matches well with developments characterized by builds and composition
(e.g.,  using sequences of neighborhoods to define builds.)
-
Adjacent neighborhoods also could merge (into villages?)
  -
This provides an orderly, composition-based growth path.
-
All this supports the use of neighborhood-based integration for systems
developed by life cycles in which composition dominates.
Pros and Cons

*(Page 369)*

### ●

Drawback to call graph–based integration testing
  -
The fault isolation problem, especially for large neighborhoods.
  -
A more subtle but closely related problem occurs.
  -
What if (when) we find a fault in a node (unit) that appears in several
neighborhoods?
  -
The adjacency matrix highlights this immediately—nodes with either a
high row sum or a high column sum will be in several neighborhoods.
  -
OK, we resolve the fault in one neighborhood.
  -
But that means changing the unit’s code in some way; so what?
-Well, it means we must test all previously tested neighborhoods
that contain the changed node!
Pros and Cons

*(Page 370)*

### ●

As the last case, a fundamental uncertainty exists in all structural testings:
  -
We assume that units integrated with respect to structural information
will exhibit correct behavior.
-
We know where we are going:
  -
we want system-level threads of behavior to be correct.
-
When we finish the integration testing based on call graph, we still have a
big step to get to system-level threads.
-
We resolve this by changing the basis from call graph information to special
forms of paths.
Pros and Cons

*(Page 371)*

### ●

Much of the progress in the development of mathematics comes from an
elegant pattern:
  -
have a clear idea of where you want to go
  -
define the concepts that take you there
-
Path-based integration testing does that.
-
When a unit executes, some path of source statements is traversed.
Suppose that a call goes to another unit along such a path.
-
At that point, control is passed from the calling unit to the called unit,
where some other path of source statements is traversed.
Path-Based Integration

*(Page 372)*

### ●

Two possibilities are available:
  -
abandon the single-entry, single-exit precept and treat such calls as
an exit followed by an entry
  -
suppress the call statement because control eventually returns to the
calling unit anyway
-
Suppression works well for unit testing, but it is not compatible with
integration testing. So how we find a better way for doing all these?
-
Refining some of the program (written in imperative languages) graph
concepts can help.
  -
Allow statement fragments to be a complete statement
  -
Statement fragments are nodes in the program graph
Path-Based Integration

*(Page 373)*

### ●

Source Node
  -
A statement fragment at which program execution begins or resumes.
  -
The first executable statement in a unit is clearly a source node.
  -
Source nodes also occur immediately after nodes that transfer control to
other units.
-
Sink Node
  -
A statement fragment at which program execution terminates.
  -
The final executable statement in a program is clearly a sink node.
  -
Also statements that transfer control to other units.
Path-Based Integration - New and Extended Concepts

*(Page 374)*

### ●

Module Execution Path
  -
A sequence of statements that begins with a source node and ends with
a sink node, with no intervening sink nodes.
  -
So now, program graphs have multiple source and sink nodes.
  -
This would greatly increase the complexity of unit testing, but integration
testing presumes unit testing is complete.
Path-Based Integration - New and Extended Concepts

*(Page 375)*

### ●

Message
  -
A programming language mechanism
  -
lets one unit transfer control to another unit and
  -
receive a response from the other unit
  -
Depending on the programming language, messages can be
-
procedure calls
-
function references
-
usual messages in an object-oriented programming language
-
We follow the convention that the unit that receives a message (the message
destination) always eventually returns control to the message source (synchronous).
-
Messages can pass data to other units.
Path-Based Integration - New and Extended Concepts

*(Page 376)*

### ●

MM-Path
  -
An interleaved sequence of module execution paths (MEP) and messages.
  -
Sequences of MEPs that include transfers of control among separate units.
-
In traditional software
  - “MM” is  module–message
-
In OO software
  - “MM” is method–message
  -
These transfers are by messages, therefore,
-
MM-paths always represent feasible execution paths
-
These paths cross unit boundaries
Path-Based Integration - New and Extended Concepts

*(Page 377)*

### Path-Based Integration - New and Extended Concepts

Hypothetical MM-path across three units

*(Page 378)*

### ●

MM-path graph
  -
Given a set of units, it is the directed graph.
  -
Nodes are MEPs.
  -
Edges correspond to messages and returns from one unit to another.
-
MM-path graphs are defined with respect to a set of units.
-
Supports composition of units and composition-based integration testing.
-
We can even compose down to the level of individual module execution
paths, but that is probably more detailed than necessary.
Path-Based Integration - New and Extended Concepts

*(Page 379)*

### ●

We should consider the relationships among
  -
MEPs
  -
program paths
  -
DD-paths
  -
and MM-paths
-
A program path is a sequence of DD-paths
-
An MM-path is a sequence of module execution paths
Path-Based Integration - New and Extended Concepts

*(Page 380)*

### ●

There is no simple relationship between DD-paths and module execution
paths.
-
Either might be contained in the other
-
but more likely, they partially overlap
-
MM-paths implement a function that transcends unit boundaries
-
So one relationship exists:
  -
consider the intersection of an MM-path with a unit
  -
The MEPs in such an intersection are an analog of a slice with respect to
the (MM-path) function.
  -
In other words, the MEPs in such an intersection are the restriction of the
function to the unit in which they occur.
Path-Based Integration - New and Extended Concepts

*(Page 381)*

### Path-Based Integration - New and Extended Concepts

1
2
3
4
5
6
1
2
3
4
1
2
3
4
5
(Module A)
(Module B)
(Module C)
A1= <1,2,3,6>;   A2=<1,2,4> ; A3 = <5,6>
Module Execution Paths:        B1= <1,2> ; B2 = <3,4>
C1= <1,2,4,5> ; C2= <1,3,4,5>

*(Page 382)*

### ●

Some practical guidelines for MM-
path integration:
  -
How long (“deep” might be
better) is an MM-path? The
notion of message quiescence
(message inactivity) helps
here.
  -
Message quiescence occurs
when a unit that sends no
messages is reached (module
C in the figure).
Path-Based Integration - New and Extended Concepts

*(Page 383)*

### ●

This could be taken as a “midpoint” of
an MM-path—the remaining
execution consists of message
returns.
-
It is helpful, but what if there are two
points of message quiescence?
  -
Maybe a better answer is to take
the longer of the two, or,
  -
if they are of equal depth, the
latter of the two.
-
Points of message quiescence are
natural endpoints for an MM-path.
Path-Based Integration - New and Extended Concepts

*(Page 384)*

### MM-Path Complexity

Cyclomatic complexities of two MM-paths

*(Page 385)*

### ●

MM-paths are a hybrid of functional and structural testing.
  -
Functional in the sense that they represent actions with inputs and
outputs.
  -
So, all the functional testing techniques are potentially applicable.
-
Cross-check of the functional and structural approaches is consolidated
into the constructs for path-based integration testing.
-
While we avoid the pitfall of structural testing, integration testing gains a
fairly seamless junction with system testing (which we discuss in the
upcoming lecture).
Pros and Cons

*(Page 386)*

### ●

Path-based integration testing works equally well for software developed in
the traditional waterfall process or with one of the composition-based
alternative life cycle models.
-
MM-path concept also applies directly to object-oriented software.
-
Most important advantage
  -
It is closely coupled with actual system behavior (structural motivations
of decomposition and call graph–based integration are not).
-
The advantages come at a price
  -
more effort is needed to identify the MM-paths.
-
This effort is probably compensated by the elimination of stub and driver
development.
Pros and Cons

*(Page 387)*

### Example

Functional decomposition of integrationNextDate
Call graph of integrationNextDate

*(Page 388)*

### Example

MM-path for May 27, 2012

*(Page 389)*

### ●

What is the significant improvement of MM-paths as a basis for integration testing?
  -
Their exact representation of dynamic software behavior.
  -
They are also the basis for present research in data flow (define/use)
approaches to integration testing.
-
MM-paths integration approach requires extra effort. So, what to do if it didn’t look
efficient in some cases?
  -
Take a fallback position, use call graphs.
Conclusions and Recommendations
Comparison of Integration Testing Strategies

*(Page 390)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 13.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
System Testing

*(Page 391)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.

*(Page 392)*

---

## Lecture 16

### A note for students

-
This material must be assumed neither as a replacement for your notes,
which you should take during the lectures, nor as a replacement for the
required reading texts, which have been presented in the further reading
section, but only as a guideline for preparation for class and for further
studies.
-
The slides are mainly adaptation and summarization from Jorgensen (2014)
[Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s
Approach. CRC Press, Taylor & Francis Group.], but I also used the
resources you can find at the end of these slides.

*(Page 394)*

### Contents

-
System Testing
  -
Functional Testing
-Thread-based Testing
  -
Nonfunctional Testing
-Stress Testing
-
References

*(Page 395)*

### ●System level is closest to everyday experience if we compare it

to the other two levels.
-System Testing Objective:
  - To demonstrate correct behavior!
  - And to find where it departs our expectations.
-When we do it?
  - Usually before a delivery deadline.
Overview

*(Page 396)*

### ●

Atomic System Function (ASF)
  - It is an action that is observable at the system level in terms of
port input and output events.
  - It is based on:
-Thread concept
-
Thread-based system testing
  - Closely coupled with requirements specification.
  - It uses the symbiosis between specification-based and code-based
testing.
Overview

*(Page 397)*

### ●What are threads?

  - hard to define!
Threads
Several views of a thread
A scenario of normal usage
A system-level test case
A stimulus/response pair
Behavior that results from a sequence of system-level inputs
An interleaved sequence of port input and output events
A sequence of transitions in a state machine description of the system
An interleaved sequence of object messages and method executions
A sequence of machine instructions
A sequence of source instructions
A sequence of MM-paths
A sequence of ASFs

*(Page 398)*

### ●Let us see how it works through an example: an ATM system

Threads
The Simple ATM (SATM) terminal
https://www.houseoftesting.com/atm-machines

*(Page 399)*

### SATM screens


*(Page 400)*

### ●

Some candidate threads in our SATM system:
  -
Entry of a digit
  -
Entry of a personal identification number (PIN)
  -
A simple transaction:
-ATM card entry
-PIN entry
-select transaction type (deposit, withdraw)
-present account details (checking or savings, amount)
-conduct the operation
-report the results
Thread Possibilities

*(Page 401)*

### 1. A screen requesting PIN digits.

2. An interleaved sequence of digit keystrokes and screen responses.
3. The possibility of cancellation by the customer before the full PIN is
entered.
4. A system disposition: a customer has three chances to enter the correct
PIN.
-
Once a correct PIN has been entered,
  -
the user sees a screen requesting the transaction type; otherwise,
  -
a screen advises the customer that the ATM card will not be returned,
and no access to ATM functions is provided.
Thread Possibilities

*(Page 402)*

### ●

Atomic System Function (ASF)
  -
An action that is observable at the system level in terms of port input and
output events.
  -
In an event-driven system, ASFs are separated by points of event
quiescence
-when a system is (nearly) idle, waiting for a port input event to trigger
further processing.
-
Event quiescence has an interesting Petri net insight (if you are interested,
consult the resources of the module    .)
Thread Definitions

*(Page 403)*

### ●

ASF graph of the system
  -
is the directed graph in which nodes are ASFs and edges represent
sequential flow.
-
Source ASF
  -
is an ASF that appears as a source node in the ASF graph of a system.
-
Sink ASF
  -
is an ASF that appears as a sink node in the ASF graph.
Thread Definitions

*(Page 404)*

### ●

In the SATM system, the card entry ASF is a source ASF, and the session
termination ASF is a sink ASF.
-
Notice that intermediary ASFs could never be tested at the system level by
themselves—they need the predecessor ASFs to “get there.”
-
System thread
  -
is a path from a source ASF to a sink ASF in the ASF graph of a system.
Thread Definitions

*(Page 405)*

### ●Recall the notion of a basis of a vector space.

-Instead of anticipating all the variations in scores of
requirements specification methods system testing can use a
basis set of requirements specification constructs:
  - Data
  - Actions
  - Devices
  - Events
  - Threads
Basis Concepts for Requirements Specification

*(Page 406)*

### ●

For many systems, the data-centered view dominates.
-
Entity/relationship (E/R) models are the most common choice at the
highest level (what about other forms of data storage and
manipulation?).
-
These systems are often developed in terms of CRUD actions
  - Create
  - Retrieve
  - Update
  - Delete
Basis Concepts for Requirements Specification (Data)

*(Page 407)*

### ●Sometimes threads can be identified directly from the data

model.
-Also, some data are read but not written (e.g., PIN)
-Read-only data must be part of the system initialization process.
-If not, there must be threads that create such data.
-Read-only data is therefore an indicator of source ASFs.
Basis Concepts for Requirements Specification (Data)

*(Page 408)*

### ●

Action-centered modeling is still a common requirements specification form.
-
Actions have inputs and outputs, and these can be either data or port
events.
-
Some methodology-specific synonyms for actions:
  -
Transform
  -
Data transform
  -
Control transform
  -
Process
  -
Activity
  -
Task
  -
Method
  -
Service
Basis Concepts for Requirements Specification (Actions)

*(Page 409)*

### ●

Every system has port devices.
-
These are the sources and destinations of system-level inputs and outputs (port events).
-
Ports and port devices are slightly different than each others.
  -
Technically, a port is the point at which an I/O device is attached to a system
-
serial and parallel ports
-
network ports
-
telephone ports
  -
Physical actions (keystrokes and light emissions from a screen) occur on port
devices.
  -
They are translated from physical to logical (or logical to physical) forms.
  -
In the absence of actual port devices, much of system testing can be accomplished
by “moving the port boundary inward” to the logical instances of port events. (writing
to PDF!)
-
We use the term “port” to refer to port devices.
Basis Concepts for Requirements Specification (Devices)

*(Page 410)*

### ●

Event characteristic:
  -
Has some characteristics of data and some of actions
  -
It is a system-level input (or output) that occurs on a port device.
  -
Similar to data, events can be inputs to or outputs of actions.
  -
Can be discrete (e.g., keystrokes)
  -
Can be continuous (e.g., temperature, altitude, or pressure)
-
Discrete events necessarily have a time duration
  -
this can be a critical factor in real-time systems.
-
We can imagine input events as destructive read-out data,
-
But it is a stretch to imagine output events as destructive write operations.
Basis Concepts for Requirements Specification (Events)

*(Page 411)*

### ●Events are similar to actions.

-They are the translation point between real-world physical
events and internal logical manifestations of these.
-Port input events are physical-to-logical translations.
-Port output events are logical-to-physical translations.
-System testers should focus on the physical side of events.
-Logical side is the focus of integration testers.
Basis Concepts for Requirements Specification (Events)

*(Page 412)*

### ●

The least frequently used of the five fundamental constructs.
-
It usually falls to the tester to find them in the interactions among the
data, events, and actions.
-
When threads appear in a requirements specification?
  - When rapid prototyping is used in conjunction with a scenario
recorder.
-
It is easy to find threads in control models.
  - But they are models, not the reality of a system!
Basis Concepts for Requirements Specification (Threads)

*(Page 413)*

### ●

An E/R model of our basis concepts (All
relationships are many-to-many):
  -
Data and Events are inputs to or
outputs of the Action entity.
  -
The same event can occur on several
ports, and typically many events occur
on a single port.
  -
An action can occur in several threads,
and a thread is composed of several
actions.
-
This diagram demonstrates some of the
difficulty of system testing.
-
Testers must use events and threads to
ensure that all the many-to-many
relationships among the five basis concepts
are correct.
Basis Concepts for Requirements Specification
(Relationships among Basis Concepts)
E/R model of basis concepts

*(Page 414)*

### ●

Finite state machine models of the show
system testing threads efficiently depending
on the system context.
-
At the high level
  -
states correspond to stages of
processing.
  -
transitions are caused by abstract logical
(instead of port) events.
-
In SATM, for example:
  -
The card entry “state” would be
decomposed into lower levels that deal
with details such as jammed cards, cards
that are upside down, stuck card rollers.
Model-Based Threads
Uppermost level SATM finite state machine

*(Page 415)*

### Model-Based Threads


*(Page 416)*

### Model-Based Threads


*(Page 417)*

### Model-Based Threads


*(Page 418)*

### ●

The system testing ideas we discussed have been based on specification-based, or
behavioral, requirements.
-
To generalize, nonfunctional testing refers to how well a system performs its
functional requirements.
-
Many nonfunctional requirements are categorized onto “-abilities”:
  -
Reliability
  -
Maintainability
  -
Scalability
  -
Usability
  -
Compatibility
  -
...
-
While many practitioners have clear ideas on the meaning of the -abilities in their product
domains, there is not much standardization of either the terms or the techniques.
Nonfunctional System Testing

*(Page 419)*

### ●

It is also called
  - performance testing
  - capacity testing
  - load testing (I disagree! Load testing considers an upper limit
while stress tests beyond the limit.)
-
One of the most common important form of nonfunctional testing (in
my opinion, along with security testing.)
-
Stress testing techniques are application dependent.
Stress Testing Strategies

*(Page 420)*

### ●

Common strategies to stress testing:
  - Compression
  - Replication
  - Mathematical Approaches
-Queuing theory
-Reliability models
-Simulation
Stress Testing Strategies

*(Page 421)*

### Systems Testing – Last Comments

Is that all?
Over 50 different types of system testing!
Usability Testing
Recovery Testing
Migration Testing
Hardware/Software Testing
Installation Testing
Security Testing
And more!
-----------------------------------
Difficulties
Time/Budget
Communication (Team, Stakeholders, Regulation, ...)
Time to Market
And more!
So, What to do?

*(Page 422)*

### A Comparison between Unit, Integration, and System Testing


*(Page 423)*

### ●Study an example that illustrates ASF testing in

your textbook (Section 14.10 of Chapter 14).
Practice at Home!

*(Page 424)*

### Activities and Next Week Topic

-
This Lecture
  -
Jorgensen (2014): Chapter 14.
  -
Consult the other introduced references.
  -
Search online about the topics that we discussed this week and expand
your knowledge about software testing in general.
  -
Explore UKH library, the computing section, and make yourself
familiarized with the resources related to this module.
-
Next Lecture
  -
Acceptance Testing (Customer Acceptance)

*(Page 425)*

### References / Further Readings

-
The lectures have been mainly adapted from the module textbooks:
  -
Jorgensen, P. C. 2014. Software Testing and Analysis, A Craftsman’s Approach.
CRC Press, Taylor & Francis Group.
-
Other resources that have been used:
  -
Ammann, P. and Offutt, J, 2008. Introduction to Software Testing, UK: Cambridge
University Press.
  -
Myers, G. J., 2012. The Art of Software Testing. John Wiley & Sons.
  -
Pezzè, M. and Young, M. 2008. Software Testing and Analysis: Process,
Principles, and Techniques. John Wiley & Sons.
  -
https://pg-p.ctme.caltech.edu/blog/coding/system-testing-in-software-testing-type
s-tips#:~:text=Time%20and%20resource%20constraints.,can%20cause%20signi
ficant%20time%20delays
.

*(Page 426)*

---
