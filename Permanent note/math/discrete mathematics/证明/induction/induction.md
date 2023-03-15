---
aliases: [mathematical induction]
sr-due: 2023-03-25
sr-interval: 46
sr-ease: 230
---
#discrete__mathematics #review #todo 拆分

# ordinary induction

## the induction principle

Let $P$ be a predicate on nonnegative integers. If

1. $P(0)$ is true
2. $P(n)$ IMPLIES $P(n+1)$ for all nongenerative integers $n$
   then,
   $P(m)$ is true for all nonnegative integers $m$

## induction rule

$\frac{P(0), \forall n \in \mathbb{N}.P(n) \quad IMPLIES \quad P(n+1)}{\forall m \in \mathbb{N}.P(m)}$

## induction proof template

1. State that the proof uses induction
2. Define an appropriate predicate $P(n)$, $P(n)$ is *induction hypothesis*
3. Prove that $P(0)$ is true
4. Prove that $P(n)$ implies $P(n+1)$ for every nonnegative integer $n$
5. Invoke induction

# strong induction

## aim

Proving that a predicate is true for all nonnegative integers.

## principles

Let $P$ be a predicate on nonnegative integers. If

1. $P(0)$ is true
2. For all $n$ in $\mathbb{N}, P(0),P(1),...P(n)$  together imply $P(n+1)$
   then $P(m)$ is true for all $m \in \mathbb{N}$
   ==You can assume a stronger set(from ​==​==$P(0)$==​==​ to ​==​==$P(n)$==​==​ are all true) of hypotheses==

## Rule

$\frac{P(0), [\forall k \leq n \in \mathbb{N}. P(k)] \quad IMPLIES \quad P(n+1)}{\forall m \in \mathbb{N}.P(m)}$

==Any proof by strong induction can be reformatted into a proof using ordinary induction. As the same, any well ordering proof can automatically be reformatted into an induction form. They are simply different formats for presenting the same mathematical reasoning.==

## invariant

Hold for initial state and preserved for every single step but does not hold at special states. This means that you can’t reach it.
