---
title: "laziness"
date: 2024-03-19
draft: false
description: "a description"
summary: "Discover the benefits of laziness, including the ability to work with infinite structures, optimize resource usage, and promote modular code design."
showHero: true
heroStyle: "big"
showSummary: true
showTaxonomies: true
slug: "laziness"
tags: ["laziness", "recursion", "concepts"]
---
<h2 class="mt-0">∞</h2>
{{< spotify type="track" id="58XoFUU8BAw3HIfMLSIxiL" width="auto" height="100" >}}
{{< katex >}}

# Explaining laziness with Haskell

Laziness, or non-strict evaluation, is a programming strategy where expressions
are only evaluated when their values are necessary. This allows for potentially
infinite data structures, efficient resource utilization, and a more modular
approach to programming. Haskell is a language fundamentally designed around the
concept of laziness.

**Unlike strict languages, which evaluate expressions eagerly, Haskell delays
computation until a value is explicitly required.**

## The Fibonacci definition

The Fibonacci sequence is a series of numbers where each number is the sum of
the two preceding ones, starting from 0 and 1. In Haskell, we can elegantly
define this infinite sequence using laziness:

```haskell
fibonacci :: [Integer]
fibonacci = 0 : 1 : zipWith (+) fibonacci (tail fibonacci)
```

### How it works

- The `fibonacci` function produces an infinite list of Fibonacci numbers.
- The expression `0 : 1 : ...` starts the list with the base elements 0 and 1.
- `zipWith (+) fibonacci (tail fibonacci)` calculates the rest of the sequence. 
  - `zipWith` takes paired elements from 'fibonacci' and its tail (the list
    without the first element), sums them using `(+)`, and appends the result to
    the list.
    
## Action

Because of laziness, Haskell doesn't try to compute the entire infinite list at
once. Let's visualize:

```
1. [0, 1, <lazy>]
2. [0, 1, 1, <lazy>]
3. [0, 1, 1, 2, <lazy>] 
... and so on
```

Haskell generates only the elements we need, when we need them.

## Benefits

- **Infinite structures** :: We can work with infinite data structures without
  memory issues.
- **Efficiency** :: Computations are performed only when necessary.
- **Modularity** :: Functions can be composed easily without concerns about
  evaluation order.
