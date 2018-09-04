---
use_math: true
title: Sets
---

# Sets

>Definition:
>
>A **set** is a collection of objects. If the object $x$ is in the set $S$, we write $x \in S$, and say that $x$ is an element of the set $S$.

This might seem like a vague definition, but that's because sets are very flexible. A set can be a collection of anything: numbers, movies, food items, other sets. We'll almost always just deal with sets that contain numbers. 

The **empty set**, denoted by $\emptyset$, doesn't contain anything. There are no elements in this set. (We avoid saying "it's the set that contains nothing," because we might be tempted to think of "nothing" itself has an object, in which case the set containing nothing certainly contains something!) 

$\mathbb{N}$, $\mathbb{Z}$, $\mathbb{Q}$, and $\mathbb{R}$ are sets. Each contains the corresponding numbers we described earlier.

We call a set $B$ a **subset** of a set $A$, and write $B \subset A$, if everything element of $B$ is also in $A$. That is, if $x \in B$, then $x\in A$. If $B$ contains an element that $A$ does not, then $B$ is not a subset of $A$. Convince yourself that for any set $A$, we have that $\emptyset \subset A$ and $A \subset A$.

We can then see that $\mathbb{N}\subset \mathbb{Z}$. Choose any natural number, and it is also an integer. However, it is not true that $Z \subset \mathbb{N}$. For example, $-1$ is an integer, but it is not a natural number. So $\mathbb{Z}$ has elements that $\mathbb{N}$ doesn't have.

