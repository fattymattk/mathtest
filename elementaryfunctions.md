---
use_math: true
title: elementary functions
---

# Elementary Functions

Here we will define some common functions with which we should be familiar.

## Polynomials

Polynomials are functions $p: \mathbb{R} \rightarrow \mathbb{R}$ that take the form

$$p(x) = a_n x^n + a_{n-1} x^{n-1} + ... + a_2 x^2 + a_1 x + a_0.$$

The polynomial $p$ here is said to have **degree** $n$, i.e. the degree is the greatest power to which $x$ is raised.

A **root**, or **zero**, of a polynomial $p$ is a number $a$ such that $p(a) = 0$. This can be interpreted as the values where the graph intersects the $x$-axis.

There are a few things we can say about polynomials:

*A polynomial of degree $n$ has at most $n$ real roots.

*The product, sum, and difference of any two polynomials is a polynomial.

*If $p(a) = 0$ (if $a$ is a root of $p$), then $p(x) = (x-a)q(x)$ for some polynomial $q$ that is degree $1$ less than $p$.


In particular, if the degree of $p$ is $0$, then $p(x) = c$ for some real number $c$, which means $p$ is a **constant** function. Constant functions are those that return the same output no matter what input we give it.

If the degree of $p$ is $1$, then $p(x) = mx+b$ for some real numbers $m$ and $b$, with $m \neq 0$. In this case, we say that $p$ is a **linear** function. We call $m$ the **slope** of $p$, and we call $b$ the $y$**-intercept**.

If the degree of $p$ is $2$, then $p(x) = ax^2 + bx + c$ for some real numbers $a$, $b$, and $c$, with $a\neq 0$. We call $p$ a **quadratic function**. You should be familiar with the quadratic formula, which gives us an explicit way to determine the roots of $p$:

$$ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$$.

The $\pm$ here indicates that there are possibly two roots: one being if we take this symbol to mean $+$ and one if we take it to mean $-$ in the above equation.

Since we cannot take the square root of negative numbers, a quadratic function has no roots of $b^2 -4ac <0$. In this case, the graph is such that it always lies completely above or below the $x$-axis. If $b^2-4ac=0$, then there is only one root, and the graph just touches the $x$-axis in one spot (the vertex touches it). If $b^2-4ac > 0$, then there are two roots and the graph intersects the $x$-axis in two places. 

We can continue giving names, such as cubic, quartic, quintic, etc, but the ones we've named so far are the important ones, and we can refer to the rest by their degree rather than their name.

`polynomial division?`


## Power Functions
