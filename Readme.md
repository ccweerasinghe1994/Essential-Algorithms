# Essential Algorithms

- [Essential Algorithms](#essential-algorithms)
  - [Chapter 1 Algorithm Basics](#chapter-1-algorithm-basics)
    - [Approach](#approach)
      - [Algorithms and Data Structures 2](#algorithms-and-data-structures-2)
      - [Pseudocode](#pseudocode)
      - [Algorithm Features](#algorithm-features)
      - [Big O Notation](#big-o-notation)
      - [Rule](#rule)
      - [Rule](#rule-1)
      - [Rule](#rule-2)
      - [Rule](#rule-3)
      - [Rule](#rule-4)
      - [Common Run Time Functions](#common-run-time-functions)
      - [Log N](#log-n)
      - [Sqrt N](#sqrt-n)
      - [N](#n)
      - [N log N](#n-log-n)
      - [N2](#n2)
      - [2N](#2n)
      - [N!](#n-1)
      - [Visualizing Functions](#visualizing-functions)
      - [Practical Considerations](#practical-considerations)
      - [Summary](#summary)
      - [Exercises](#exercises)
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

## Chapter 1 Algorithm Basics
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
### Approach 
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
and sometimes it’s the techniques they use (`recursion, decision trees, distributed
algorithms`). At a high level, these groupings may seem arbitrary, but when you
read about the algorithms, you’ll see that they fit together.

In addition to those categories, many algorithms have underlying themes that
cross chapter boundaries. For example, tree algorithms (Chapters 10, 11, and 12)
tend to be `highly recursive` (Chapter 9). `Linked lists` (Chapter 3) can be used to
build `arrays` (Chapter 4), `hash tables` (Chapter 8), `stacks` (Chapter 5), and `queues`
(Chapter 5). The ideas of `references` and `pointers` are used to build `linked lists`
(Chapter 3), `trees` (Chapters 10, 11, and 12), and `networks` (Chapters 13 and 14). As
you read, watch for these common threads. Appendix A summarizes common
strategies programs use to make these ideas easier to follow.

#### Algorithms and Data Structures 2
An `algorithm` is a recipe for performing a certain `task`. A `data structure` is a way
of `arranging data` to make solving a particular `problem` easier. A `data structure` could be a way of arranging `values` in an `array`, a `linked list` that connects items
in a certain `pattern`, a `tree`, a `graph`, a `network`, or something even more `exotic`.

`Algorithms` are often closely tied to `data structures`. For example, the edit
distance algorithm described in Chapter 15, `“String Algorithms,”` uses a `network` to determine how similar two strings are. The algorithm is tied closely to
the `network` and won’t work without it. Conversely, the `algorithm` builds and
uses the `network`, so the `network` isn’t useful (or really even built) without the
`algorithm`.

Often an `algorithm` says, *“Build a certain data structure and then use it in a
certain way*.” The algorithm can’t exist without the data structure, and there’s no
point in building the data structure if you don’t plan to use it with the algorithm.

#### Pseudocode 
#### Algorithm Features 
#### Big O Notation 
#### Rule 
#### Rule 
#### Rule
#### Rule 
#### Rule 
#### Common Run Time Functions
#### Log N 
#### Sqrt N 
#### N 
#### N log N 
#### N2 
#### 2N 
#### N! 
#### Visualizing Functions 
#### Practical Considerations 
#### Summary 
#### Exercises
## Chapter 2 Numerical Algorithms
## Chapter 3 Linked Lists
## Chapter 4 Arrays
## Chapter 5 Stacks and Queues
## Chapter 6 Sorting
## Chapter 7 Searching
## Chapter 8 Hash Tables
## Chapter 9 Recursion
## Chapter 10 Trees
## Chapter 11 Balanced Trees
## Chapter 12 Decision Trees
## Chapter 13 Basic Network Algorithms
## Chapter 14 More Network Algorithms
## Chapter 15 String Algorithms
## Chapter 16 Cryptography
## Chapter 17 Complexity Theory
## Chapter 18 Distributed Algorithms
## Chapter 19 Interview Puzzles
## Appendix A Summary of Algorithmic Concepts
## Appendix B Solutions to Exercises
## Glossary
## Index