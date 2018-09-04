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

Similarly, we can see that $\mathbb{Z} \subset \mathbb{Q}$ and $\mathbb{Q} \subset \mathbb{R}$.

As an exercise, show that if $B \subset A$ and $C \subset B$, then $C \subset A$. Conclude, for example, that $\mathbb{Z}$ and $\mathbb{N}$ are subsets of $\mathbb{R}$.

Let $A$ and $B$ be sets. The **union** of $A$ and $B$, denoted by $A \cup B$, is defined to be the set of elements that are in $A$ **or** are in $B$. The **intersection** of $A$ and $B$, denoted by $A \cap B$, is defined to be the set of elements that are in $A$ **and** are in $B$.

Two sets are equal if they contain the same elements. Put another way, for sets $A$ and $B$, we write $A=B$ if and only if every element in the set $A$ is also in set $B$, and every element in the set $B$ is also in set $A$. Convince yourself that $A=B$ if and only if $A \subset B$ and $B \subset A$.

## Set Builder Notation

If a set does not have many elements in it, we can define it just by listing its elements. Defining $A = \{2,3,7\}$, we say that $A$ is the set that contains the numbers $2$, $3$, and $7$ (and nothing else). It's important to note that order doesn't matter here. If $B = \{3,2,7\}$, then $A=B$.

We can also define a set by describing the properties each element of the set has. If $C$ is the set that contains all real numbers less than or equal to $2$, then we write $C = \{x \in \mathbb{R} | x \leq 1 \}$. This can be read as "$C$ is the set equal to the set of all real $x$ values such that $x \leq 1$."

Another example: let $D=\{x \in \mathbb{Q} | x > \sqrt{2} \mbox{ or } x < - \sqrt{2} \}$. The set $D$ then contains all rational numbers that are greater than $\sqrt{2}$ or less than $-\sqrt{2}$.


## Intervals

Intervals are a special type of subset of the real numbers. An interval can be **open**, **closed**, or neither.

> Definition:
>
>Let $a$ and $b$ be real numbers with $a < b$. Then the set denoted by $(a,b)$ is defined to be $\{x \in \mathbb{R} | a < x < b \}$, and we call it an **open interval**.

> Definition:
>
>Let $a$ and $b$ be real numbers with $a \leq b$. Then the set denote by $\[a,b\]$ is defined to be $\{x \in \mathbb{R} | a \leq x \leq b \}$, and we call it a **closed interval**.

So closed intervals contain their endpoints, where as open intervals do not.

Open intervals have the nice property that if $x \in (a,b)$, then there exists $y \in (a,b)$ such that $y < x$, and there also exists $z \in (a,b)$ such that $ x < z$. So all elements in an open interval are "surrounded" by other elements in the interval. Closed intervals don't have this property, since $a$ and $b$ are both in the closed interval $\[a,b\]$, but there are not elements in this interval that are less that $a$, and there are no elements in this  interval that are greater than $b$. So we can't think of all the elements in a closed interval as being "surrounded."

## Infinity

This is a good time to mention the mysterious concept of infinity. We do not think of infinity as a real number. It is more of a concept that we get to think about than a number that we get to play around with. We will think of infinity as the concept of being greater than all the real numbers, but not a real number itself.

Therefore, we will define the set $(a,\infty)$ as $\{x \in \mathbb{R} | x > a \}$. We could also think of it as all the real numbers between $a$ and infinity, since all real numbers are less than infinity.

Similarly, we will think of negative infinity as something that's less than all the real numbers, but not a real number itself. We can then define $(-\infty, b)$ as $\{x \in \mathbb{R} | x < b \}$.

The sets $(a,\infty)$ and $(-\infty,b)$ are both open. They still have the property that each element in them are surrounded on both sides by other elements of the set.

Some sets are neither open or closed. For example, the set $\[a,b)$ is naturally defined to be $\{ x \in \mathbb{R} | a \leq x < b \}$. It is neither open nor closed.

There are other intervals we can write, such as $\(a,b\]$, $(-\infty,b\]$, and $\[a, \infty)$. It should be clear how to extend the above definitions to these sets.

Lastly, the set $\mathbb{R}$ can also be written as $(-\infty, \infty)$. Think about why.



