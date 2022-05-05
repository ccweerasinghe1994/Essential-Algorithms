# 🛩️Essential Algorithms🛩️

- [🛩️Essential Algorithms🛩️](#️essential-algorithms️)
  - [🚨Chapter 1 Algorithm Basics🚨](#chapter-1-algorithm-basics)
    - [🚁Approach](#approach)
      - [🗼Algorithms and Data Structures 2](#algorithms-and-data-structures-2)
      - [🗼Pseudocode](#pseudocode)
      - [🗼Algorithm Features](#algorithm-features)
      - [🗼Big O Notation](#big-o-notation)
  - [#### 🗼Rule](#-rule)
      - [🗼Rule](#rule)
  - [#### 🗼Rule](#-rule-1)
  - [#### 🗼Rule](#-rule-2)
  - [#### 🗼Rule](#-rule-3)
      - [🗼Common Run Time Functions](#common-run-time-functions)
      - [🗼Log N](#log-n)
      - [🗼Sqrt N](#sqrt-n)
      - [🗼N](#n)
      - [🗼N log N](#n-log-n)
      - [🗼N2](#n2)
      - [🗼2N](#2n)
      - [🗼N!](#n-1)
      - [🗼Visualizing Functions](#visualizing-functions)
      - [🗼Practical Considerations](#practical-considerations)
      - [🗼Summary](#summary)
      - [🗼Exercises](#exercises)
  - [Chapter 2 Numerical Algorithms](#chapter-2-numerical-algorithms)
  - [Chapter 3 Linked Lists](#chapter-3-linked-lists)
  - [Chapter 4 Arrays](#chapter-4-arrays)
  - [Chapter 5 Stacks and Queues](#chapter-5-stacks-and-queues)
  - [Chapter 6 Sorting](#chapter-6-sorting)
  - [Chapter 7 Searching](#chapter-7-searching)
  - [Chapter 8 Hash Tables](#chapter-8-hash-tables)
  - [Chapter 9 Recursion](#chapter-9-recursion)
  - [Chapter 10 Trees](#chapter-10-trees)
  - [Chapter 11 Balanced Trees](#chapter-11-balanced-trees)
  - [Chapter 12 Decision Trees](#chapter-12-decision-trees)
  - [Chapter 13 Basic Network Algorithms](#chapter-13-basic-network-algorithms)
  - [Chapter 14 More Network Algorithms](#chapter-14-more-network-algorithms)
  - [Chapter 15 String Algorithms](#chapter-15-string-algorithms)
  - [Chapter 16 Cryptography](#chapter-16-cryptography)
  - [Chapter 17 Complexity Theory](#chapter-17-complexity-theory)
  - [Chapter 18 Distributed Algorithms](#chapter-18-distributed-algorithms)
  - [Chapter 19 Interview Puzzles](#chapter-19-interview-puzzles)
  - [Appendix A Summary of Algorithmic Concepts](#appendix-a-summary-of-algorithmic-concepts)
  - [Appendix B Solutions to Exercises](#appendix-b-solutions-to-exercises)
  - [Glossary](#glossary)
  - [Index](#index)

## 🚨Chapter 1 Algorithm Basics🚨

---

Before you jump into the study of `algorithms`, you need a little background. To
begin with, you need to know that, simply stated, an algorithm is a `recipe for getting something done`. It defines the steps for performing a task in a certain way.
That definition seems simple enough, but no one writes algorithms for
performing extremely simple tasks. No one writes instructions for how to
access the fourth element in an array. It is just assumed that this is part of the
definition of an array and that you know how to do it (if you know how to use
the programming language in question).
Normally, people write algorithms only for `difficult` tasks. Algorithms explain
how to find the `solution` to a complicated algebra problem, how to find the shortest path through a `network` containing thousands of streets, or how to find the
best mix of hundreds of investments to optimize profits.
This chapter explains some of the basic algorithmic concepts you should
understand if you want to get the most out of your study of algorithms.
It may be tempting to skip this chapter and jump to studying specific algorithms, but you should at least skim this material. Pay close attention to the section “Big O Notation,” because a good understanding of run time performance
can mean the difference between an algorithm performing its task in seconds,
hours, or not at all.

### 🚁Approach

---

To get the most out of an algorithm, you must be able to do more than simply
follow its steps. You need to understand the following:

`The algorithm’s behavior` Does it find the best possible solution, or does it
just find a good solution? Could there be multiple best solutions? Is there a
reason to pick one “best” solution over the others?

`The algorithm’s speed` Is it fast? Slow? Is it usually fast but sometimes slow
for certain inputs?

`The algorithm’s memory requirements` How much memory will the algorithm
need? Is this a reasonable amount? Does the algorithm require billions of
terabytes more memory than a computer could possibly have (at least today)?

`The main techniques the algorithm uses` Can you reuse those techniques to
solve similar problems?

This book covers all of these topics. It does not, however, attempt to cover
every detail of every algorithm with mathematical precision. It uses an intuitive
approach to explain algorithms and their performance, but it does not analyze
performance in rigorous detail. Although that kind of proof can be interesting,
it can also be confusing and take up a lot of space, providing a level of detail
that is unnecessary for most programmers. This book, after all, is intended
primarily for programmers who need to get a job done.

This book’s chapters group algorithms that have related themes. Sometimes
the theme is the task that they perform (`sorting, searching, network algorithms`),
sometimes it’s the data structures they use (`linked lists, arrays, hash tables, trees`),
and sometimes it’s the techniques they use (`recursion, decision trees, distributed algorithms`). At a high level, these groupings may seem arbitrary, but when you
read about the algorithms, you’ll see that they fit together.

In addition to those categories, many algorithms have underlying themes that
cross chapter boundaries. For example, tree algorithms (Chapters 10, 11, and 12)
tend to be `highly recursive` (Chapter 9). `Linked lists` (Chapter 3) can be used to
build `arrays` (Chapter 4), `hash tables` (Chapter 8), `stacks` (Chapter 5), and `queues`
(Chapter 5). The ideas of `references` and `pointers` are used to build `linked lists`
(Chapter 3), `trees` (Chapters 10, 11, and 12), and `networks` (Chapters 13 and 14). As
you read, watch for these common threads. Appendix A summarizes common
strategies programs use to make these ideas easier to follow.

#### 🗼Algorithms and Data Structures 2

---

An `algorithm` is a recipe for performing a certain `task`. A `data structure` is a way
of `arranging data` to make solving a particular `problem` easier. A `data structure` could be a way of arranging `values` in an `array`, a `linked list` that connects items
in a certain `pattern`, a `tree`, a `graph`, a `network`, or something even more `exotic`.

`Algorithms` are often closely tied to `data structures`. For example, the edit
distance algorithm described in Chapter 15, `“String Algorithms,”` uses a `network` to determine how similar two strings are. The algorithm is tied closely to
the `network` and won’t work without it. Conversely, the `algorithm` builds and
uses the `network`, so the `network` isn’t useful (or really even built) without the
`algorithm`.

Often an `algorithm` says, _“Build a certain data structure and then use it in a
certain way_.” The algorithm can’t exist without the data structure, and there’s no
point in building the data structure if you don’t plan to use it with the algorithm.

#### 🗼Pseudocode

---

To make the algorithms described in this book as useful as possible, they are
first described in intuitive English terms. From this `high-level` explanation, you
should be able to implement the algorithm in most programming languages.

Often, however, an algorithm’s implementation contains petty details that
can make implementation hard. To make handling those details easier, many
algorithms are also described in `pseudocode`. Pseudocode is text that is a lot
like a `programming language` but is not really a programming language. The
idea is to give you the `structure` and `details` you would need to implement the
algorithm in code without tying the algorithm to a particular programming
language. Ideally, you can translate the pseudocode into actual code to run on
your computer.

The following snippet shows an example of pseudocode for an algorithm that
calculates the `greatest common divisor (GCD)` of two integers:

```pseudocode
/// Find the greatest common divisor of a and b.
// GCD(a, b) = GCD(b, a Mod b).
Integer: Gcd(Integer: a, Integer: b)
  While (b != 0)
    // Calculate the remainder.
    Integer: remainder = a Mod b
    // Calculate GCD(b, remainder).
    a = b
    b = remainder
  End While
// GCD(a, 0) is a.
Return a
End Gcd
```

**THE MOD OPERATOR**
_The modulus operator, which is written as Mod in the pseudocode, means the
remainder after division. For example, “13 Mod 4” is 1 because 13 divided by 4 is 3 with
a remainder of 1.
The statement “13 Mod 4” is usually pronounced “13 mod 4” or “13 modulo 4.”_

The pseudocode `starts` with a comment. `Comments` begin with the characters
`//` and extend to the end of the line.

The first actual line of code is the algorithm’s declaration. This algorithm is
called Gcd and `returns` an `integer` result. It takes two parameters named `a` and
`b`, both of which are `integers`.

---

🚨`NOTE` *Chunks of code that perform a `task`, optionally returning a `result`, are variously called `routines`, `subroutines`, `methods`, `procedures`, `sub procedures`, or `functions`*🚨

---

The code after the declaration is `indented` to show that it is part of the `method`.
The first line in the method’s body begins a `While loop`. The code indented below
the While statement is `executed` as long as the `condition` in the While statement
remains `true`.

The While loop ends with an `End While` statement. This statement isn’t strictly
necessary, because the indentation shows where the loop ends, but it provides
a reminder of what kind of block of statements is ending.

The method exits at the `Return` statement. This algorithm returns a value, so
this `Return` statement indicates which value the algorithm should return. If the
algorithm doesn’t return any value, such as if its purpose is to arrange values
or build a `data structure`, the `Return` statement isn’t followed by a return value, or
the method may have no `Return` statement.

The code in this example is fairly close to actual programming code. Other
examples may contain instructions or values described in English. In those
cases, the `instructions` are enclosed in angle brackets `(<>)` to indicate that you
need to translate the English instructions into program code.

Normally, when a `parameter` or `variable` is declared (in the Gcd algorithm,
this includes the parameters a and b and the variable remainder), its data type is
given before it followed by a `colon`, as in `Integer: remainder`. The data type may
be `omitted` for simple integer looping variables, as in `For i = 1 To 10`.

One other feature that is different from some programming languages is that
a pseudocode For loop may include a `Step statement` indicating the value by
which the `looping variable` is changed after `each trip` through the `loop`. A For
loop ends with a Next `i` statement (where i is the looping variable) to remind
you which loop is ending.

For example, consider the following `pseudocode`:

```pseudocode
For i = 100 To 0 Step -5
  // Do something...
Next i
```

This code is equivalent to the following `C#` code:

```c#
for (int i = 100; i >= 0; i -= 5)
{
  // Do something...
}
```

Both of those are equivalent to the following `Python` code:

```python
for i in range(100, -1, -5):
# Do something...
```

The pseudocode used in this book uses `If-Then-Else` statements, `Case` statements, and other statements as needed. These should be familiar to you from
your knowledge of real programming languages. `Anything else` that the code
needs is `spelled out in English`.

Many algorithms in this book are written as methods or functions that return
a result. The method’s declaration begins with the result’s data type. If a method
performs some task and doesn’t return a result, it has no data type.
The following pseudocode contains two methods:

```pseudocode
// Return twice the input value.
Integer: DoubleIt(Integer: value)
  Return 2 * value
End DoubleIt

// The following method does something and doesn't return a value.
DoSomething(Integer: values[])
  // Some code here.
...
End DoSomething
```

The `DoubleIt` method takes an `integer` as a parameter and returns an `integer`.
The code doubles the input value and returns the result.
The `DoSomething` method takes as a parameter an array of integers named values.
It performs a task and `doesn’t` `return` a result. For example, it might randomize
or sort the items in the array. (Note that this book assumes that arrays start with
the index 0. For example, an array containing three items has indices 0, 1, and 2.)
Pseudocode should be intuitive and easy to understand.

One problem with `pseudocode` is that it has `no` `compiler` to detect `errors`. As a
check of the basic algorithm and to give you some actual code to use for a reference, `C#` and `Python` implementations of many of the algorithms and exercises
are available for download on the book’s website.

#### 🗼Algorithm Features

---

A `good algorithm` must have three features: `correctness`, `maintainability`, and
`efficiency`.

Obviously, if an algorithm doesn’t solve the problem for which it was designed,
it’s not much use. If it doesn’t produce correct answers, there’s little point in
using it.

🚨`NOTE` Interestingly, some `algorithms` produce `correct` answers `only some of the time` but are still useful. For example, an algorithm may be able to give you
some information with a certain `probability`. In that case, you may be able to `rerun`
the algorithm many times to increase your confidence that the answer is correct.
Fermat’s primality test, described in Chapter 2, `“Numerical Algorithms,”` is this kind of
algorithm.🚨

If an algorithm isn’t `maintainable`, it’s `dangerous` to use in a `program`. If an
algorithm is `simple, intuitive, and elegant`, you can be confident that it is producing `correct results` and you can fix it if it doesn’t. If the algorithm is `intricate`,
`confusing`, and `convoluted`, you may have a lot of `trouble` implementing it, and
you will have even more `trouble fixing` it if a bug arises. If it’s hard to understand, how can you know if it is producing correct results?

---

🚨`NOTE`This doesn’t mean that it isn’t worth studying confusing and difficult algorithms. Even if you have trouble implementing an algorithm, you may learn a lot in the
attempt. Over time, your algorithmic intuition and skill will increase, so algorithms
you once thought were confusing will seem easier to handle. You must always test all
algorithms thoroughly, however, to make sure that they are producing correct results.🚨

---

Most developers spend a lot of effort on `efficiency`, and efficiency is certainly
important. If an algorithm produces a correct result and is simple to implement
and debug, it’s still not much use if it takes seven years to finish or if it requires
more `memory` than a computer can possibly hold.

To study an algorithm’s `performance`, computer scientists ask how its
performance changes as the `size` of the `problem` changes. If you double the
number of values the algorithm is processing, does the `run time` double? Does
it increase by a `factor` of 4? Does it increase `exponentially` so that it suddenly
takes years to finish?

You can ask the same questions about `memory usage` or any other resource
that the algorithm requires. If you double the size of the problem, does the
amount of memory required double?

You can also ask the same questions with respect to the algorithm’s `performance`
under `different circumstances`. What is the algorithm’s worst-case performance?
How likely is the worst case to occur? If you run the algorithm on a large set of
random data, what is its `average-case` `performance`?

To get a feeling for how problem size relates to performance, computer scientists use `Big O notation`, which is described in the following section.

#### 🗼Big O Notation

---

Big O notation uses a function to describe how the algorithm’s worst-case
performance relates to the problem size as the size grows very large. (This is
sometimes called the program’s asymptotic performance.) The function is written
within parentheses after a capital letter O.

For example, O(N ) 2 means that an algorithm’s run time (or memory usage or
whatever you’re measuring) increases as the square of the number of inputs N.
If you double the number of inputs, the run time increases by roughly a factor
of 4. Similarly, if you triple the number of inputs, the run time increases by a
factor of 9.

---

🚨`NOTE` Often `O(N2)` is pronounced `“order N squared.”` For example, you might
say, “The `quicksort` algorithm described in Chapter 6, `‘Sorting`,’ has a `worst-case`
performance of `order N squared`.”🚨

---

There are `five` basic `rules` for calculating an algorithm’s `Big O` notation.

1. If an algorithm performs a certain sequence of steps `f(N)` times for a mathematical function f, then it takes `O(f(N))` steps.
2. If an algorithm performs an operation that takes `O(f(N))` steps and then
   performs a second operation that takes `O(g(N))` steps for functions `f` and
   g`, then the algorithm’s total performance is` `O(f(N) g(N))`.
3. If an algorithm takes `O(f(N) + g(N))` time and the function `f(N)` is `greater`
   than `g(N)` for `large N`, then the algorithm’s performance can be `simplified`
   to `O(f(N))`.
4. If an algorithm performs an operation that takes `O(f(N))` steps, and for
   every step in that operation it performs another `O(g(N))` steps, then the
   algorithm’s total performance is `O(f(N) x g(N)) ` .
5. Ignore constant multiples. If `C` is a `constant`, ` O (Cxf(N)` is the same as
   `O(f(N))`, and `O(f(C N))` is the same as `O(f(N))`.

These rules may seem a bit formal, with all that talk of f(N) and g(N), but
they’re fairly easy to apply. If they seem confusing, a few examples should make
them easier to understand.

#### 🗼Rule
---
If an algorithm performs a certain sequence of steps f(N) times for a mathematical
function f, then it takes O(f(N)) steps.
Consider the following algorithm, written in pseudocode, for finding the
largest integer in an array:🔥

```pseudocode
Integer: FindLargest(Integer: array[])
Integer: largest = array[0]
For i = 1 To <largest index>
If (array[i] > largest) Then largest = array[i]
Next i
Return largest
End FindLargest
```
🔥The FindLargest algorithm takes as a parameter an array of integers and
returns an integer result. It starts by setting the variable largest equal to the
first value in the array.

It then loops through the remaining values in the array, comparing each to
largest. If it finds a value that is larger than largest, the program sets largest equal to that value.

After it finishes the loop, the algorithm returns largest.
This algorithm examines each of the N items in the array once, so it has O(N)
performance.
****
⚠️ **NOTE** ⚠️ Often algorithms spend most of their time in loops. There’s no way an
algorithm can execute more than a few steps with a fixed number of code lines unless
it contains some sort of loop.
Study an algorithm’s loops to figure out how much time it takes.
****
#### 🗼Rule

---
If an algorithm performs an operation that takes O(f(N)) steps and then performs a second operation that takes O(g(N)) steps for functions f and g, then
the algorithm’s total performance is O(f(N) g(N)).

If you look again at the FindLargest algorithm shown in the preceding section, you’ll see that a few steps are not actually inside the loop. The following
pseudocode shows the same steps, with their run time order shown to the right
in comments:🔥

```pseudocode
Integer: FindLargest(Integer: array[])
Integer: largest = array[0] // O(1)
For i = 1 To <largest index> // O(N)
If (array[i] > largest) Then largest = array[i]
Next i
Return largest // O(1)
End FindLargest
```
🔥
This algorithm performs one setup step before it enters its loop and then
performs one more step after it finishes the loop. Both of those steps have
performance O(1) (they’re each just a single step), so the total run time for the
algorithm is really O(1+1+N). You can use normal algebra to combine terms
to rewrite this as O(2+N).

#### 🗼Rule
---
If an algorithm takes O(f(N)+g(N)) time and the function f(N) is greater than
g(N) for large N, then the algorithm’s performance can be simplified to O(f(N)).
The preceding example showed that the FindLargest algorithm has run time
O(2+N). When N grows large, the function N is larger than the constant value
2, so O(2 N) simplifies to O(N).
Ignoring the smaller function lets you focus on the algorithm’s asymptotic
behavior as the problem size becomes very large. It also lets you ignore relatively
small setup and cleanup tasks. If an algorithm spends some time building
simple data structures and otherwise getting ready to perform a big computation, you can ignore the setup time as long as it’s small compared to the length
of the main calculation.
#### 🗼Rule
---
If an algorithm performs an operation that takes O(f(N)) steps, and for every
step in that operation it performs another O(g(N)) steps, then the algorithm’s
total performance is O(f(N)xg(N)).
Consider the following algorithm that determines whether an array contains
any duplicate items. (Note that this isn’t the most efficient way to detect duplicates.)🔥

```pseudocode
Boolean: ContainsDuplicates(Integer: array[])
// Loop over all of the array's items.
For i = 0 To <largest index>
For j = 0 To <largest index>
// See if these two items are duplicates.
If (i != j) Then
If (array[i] == array[j]) Then Return True
End If
Next j
Next i
// If we get to this point, there are no duplicates.
Return False
End ContainsDuplicates
```
🔥This algorithm contains two nested loops. The outer loop iterates over all the
array’s N items, so it takes O(N) steps.
For each trip through the outer loop, the inner loop also iterates over the N
items in the array, so it also takes O(N) steps.
Because one loop is nested inside the other, the combined performance is
O N ( ) N O(N2).
#### 🗼Rule
---
Ignore constant multiples. If C is a constant, O(Cxf(N)) is the same as O(f(N)),
and O(f(CxN)) is the same as O(f(N)).

If you look again at the ContainsDuplicates algorithm shown in the preceding
section, you’ll see that the inner loop actually performs one or two steps. It performs an If test to see if the indices i and j are the same. If they are different,
it compares array[i] and array[j]. It may also return the value True.

If you ignore the extra step for the Return statement (it happens at most only
once) and you assume that the algorithm performs both of the If statements
(as it does most of the time), then the inner loop takes 
O  (2xN) steps. Therefore,
the algorithm’s total performance is O(Nx2xN)=O(2xN^2).

Rule 5 lets you ignore the factor of 2, so the run time is O(N)^2 .
This rule really goes back to the purpose of Big O notation. The idea is to get
a feeling for the algorithm’s behavior as N increases. In this case, suppose that
you increase N by a factor of 2.

If you plug the value 2xN into the equation 2 N^2, you get the 
following:
$$
2*(2*N)^2 = 2*4*N^2 = 8*N^2
$$

This is four times the original value 2*N^2, so the run time has increased by a
factor of 4.

Now try the same thing with the run time simplified by rule 5 to O(N)^2 .
Plugging 2 N into this equation gives the following:

$$
(2*N)^2 = 4*N^2
$$

This is four times the original value N^2, so this also means that the run time
has increased by a factor of 4.

Whether you use the formula 2*N^2 or just N^2, the result is the same: increasing
the size of the problem by a factor of 2 increases the run time by a factor of 4. The
important thing here isn’t the constant; it’s the fact that the run time increases
as the square of the number of inputs N.
****
⚠️ **NOTE** ⚠️ It’s important to remember that Big O notation is just intended to give you
an idea of an algorithm’s theoretical behavior. Your results in practice may be different.Chapter 1 ■ Algorithm Basics 11
For example, suppose an algorithm’s performance is O(N), but if you don’t ignore the
constants, the actual number of steps executed is something like 100,000,000 + N.
Unless N is really big, you may not be able to safely ignore the constant.
****
#### 🗼Common Run Time Functions

---

#### 🗼Log N

---

#### 🗼Sqrt N

---

#### 🗼N

---

#### 🗼N log N

---

#### 🗼N2

---

#### 🗼2N

---

#### 🗼N!

---

#### 🗼Visualizing Functions

---

#### 🗼Practical Considerations

---

#### 🗼Summary

---

#### 🗼Exercises

---

## Chapter 2 Numerical Algorithms

---

## Chapter 3 Linked Lists

---

## Chapter 4 Arrays

---

## Chapter 5 Stacks and Queues

---

## Chapter 6 Sorting

---

## Chapter 7 Searching

---

## Chapter 8 Hash Tables

---

## Chapter 9 Recursion

---

## Chapter 10 Trees

---

## Chapter 11 Balanced Trees

---

## Chapter 12 Decision Trees

---

## Chapter 13 Basic Network Algorithms

---

## Chapter 14 More Network Algorithms

---

## Chapter 15 String Algorithms

---

## Chapter 16 Cryptography

---

## Chapter 17 Complexity Theory

---

## Chapter 18 Distributed Algorithms

---

## Chapter 19 Interview Puzzles

---

## Appendix A Summary of Algorithmic Concepts

---

## Appendix B Solutions to Exercises

---

## Glossary

---

## Index

---
