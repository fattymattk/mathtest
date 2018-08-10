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

* A polynomial of degree $n$ has at most $n$ real roots.

* If $p(a) = 0$ (if $a$ is a root of $p$), then $p(x) = (x-a)q(x)$ for some polynomial $q$ that is degree $1$ less than $p$.

* The product, sum, and difference of any two polynomials is a polynomial.

In particular, if the degree of $p$ is $0$, then $p(x) = c$ for some real number $c$, which means $p$ is a **constant** function. Constant functions are those that return the same output no matter what input we give it.

If the degree of $p$ is $1$, then $p(x) = mx+b$ for some real numbers $m$ and $b$, with $m \neq 0$. In this case, we say that $p$ is a **linear** function. We call $m$ the **slope** of $p$, and we call $b$ the $y$**-intercept**.

If the degree of $p$ is $2$, then $p(x) = ax^2 + bx + c$ for some real numbers $a$, $b$, and $c$, with $a\neq 0$. We call $p$ a **quadratic function**. You should be familiar with the quadratic formula, which gives us an explicit way to determine the roots of $p$:

$$ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}.$$

The $\pm$ here indicates that there are possibly two roots: one being if we take this symbol to mean $+$ and one if we take it to mean $-$ in the above equation.

Since we cannot take the square root of negative numbers, a quadratic function has no roots of $b^2 -4ac <0$. In this case, the graph is such that it always lies completely above or below the $x$-axis. If $b^2-4ac=0$, then there is only one root, and the graph just touches the $x$-axis in one spot (the vertex touches it). If $b^2-4ac > 0$, then there are two roots and the graph intersects the $x$-axis in two places. 

We can continue giving names, such as cubic, quartic, quintic, etc, but the ones we've named so far are the important ones, and we can refer to the rest by their degree rather than their name.

`polynomial division?`


## Power Functions

A **power function** is a function in the form $f(x) = x^a$ for some constant $a$. The domain of these kinds of functions is usually the positive real numbers, as we often get into trouble if $x<0$ (i.e. $f(x) = x^{1/2}$) or if $x = 0$ (i.e. $f(x) = x^{-1}$).

You should play around with the graph [here](https://www.desmos.com/calculator/pahpuj0gr9). See what happens for different values of $a$ and try to understand why it's happening. In particular, note the qualitative differences between the cases when $a<0$, $a=0$, $0<a<1$, $a=1$, and $a>1$.

## Exponential Functions

An **exponential function** is a function in the form $f(x) = a^x$ for $a>0$ and $a\neq 1$. While this might seem similar to power functions, it's very important to note the difference. Here, the input variable is in the exponent, while the input variable for power functions are the base. This leads to very different behaviour! Check out the graph below to see the difference between the graphs of $y = x^2$ (red) and $y=2^x$ (blue).

![Power and Exponential Functions](images/power-exponential.png "Power and Exponential Functions")

The graph can be found [here](https://www.desmos.com/calculator/ozvjuacxok).

Besides the fact that they're nothing a like for negative values of $x$, the big difference is that the exponential function grows much faster. This fact has slipped into our everyday language, as we often think of something that grows very fast as growing "exponentially".

Another clear difference is that $x^2$ is $0$ when $x=0$ and $2^x$ is $1$ when $x=0$.

You can see what the graphs of exponential functions for various values of $a$ look like [here](https://www.desmos.com/calculator/arjes7hh8y). In particular, note the behaviour of the graph as $a$ increases, and note the qualitative difference between when $a<1$ and $a>1$. Why do you think we exclude the case when $a=1$?


This is a good time to review the properties of exponential functions:

* $a^(b+c) = a^b a^c$.

* $(a^b)^c = a^{bc}$.

* $a^0 = 1$.

* $a^{-b} = \frac{1}{a^b}$.

* $a^n = a\cdot a \cdot a ... \cdot a$ ($n$ times) when $n$ is a positive integer.

* $a^{m/n} = \sqrt[n]{a^m} = (\sqrt[n]{a})^m$ when $m$ and $n>0$ are integers.

We'll take these properties to be true by definition. Also, don't forget that $a>0$ and $a\neq 1$ for all of the above.

Now a natural question to ask now is what is $a^x$ when $x$ is irrational? For integer values and rational values of $x$ we have a clear definition above. But if we want to define a function in this form with a domain that is $\mathbb{R}$, then we have to think about what happens for irrationals as well.

Very loosely speaking, we want the function to be "nice". If $x$ is irrational but close to some rational number $r$, then we want $a^x$ to be close to $a^r$. If this wasn't true, then our above graph wouldn't look so nice, as it would have weird jumps wherever there are irrational inputs (and there are a lot!).

Consider for a moment the case when $a>1$. In this situation, we have discovered from the graph that the function $f: \mathbb{R} \rightarrow \mathbb{R}$ is an **increasing** function. If $x$ is irrational, $r$ is rational, and $x>r$, then it should be true that $a^x>a^r$. Similarly, if $p$ is rational and $x<p$, then $a^x < a^p$.

So although things might be becoming less than concrete, we can define $a^x$ for irrational $x$ as the following:

>If $x$ is irrational and $p$ and $r$ are *any* rational numbers such that $p<x<r$, then for $a>1$ we have that $a^p<a^x<a^r$.

This might not seem like much of a definition, but it defines a unique number $a^x$ for any irrational $x$. In practice, if we were to try and compute it using this definition, we could only achieve some sort of approximation by choose $p$ and $r$ as close to $x$ as we need. But this shouldn't be too unsettling. We have no trouble thinking of $\pi$ as a perfectly fine number, even though there is no hope of ever knowing its full decimal expansion. So there shouldn't be much of a problem thinking of $2^{\pi}$ as a well-defined number even though we might have to approximate it as somewhere between $2^{3.141}$ and $2^{3.142}$.

You might want to think of the case for $0<a<1$. It's the same idea.

`notes: we should figure out where to do inverse functions. I'm thinking right after domain and range and before increasing and decreasing. We should define 1-1 and onto. Then we are in a situation to do the log function now.`

`think about how to deal with e. Do we want to save this for when we do derivatives? I think I'll see how that goes`

`we need to do trig and inverse trig. also, we should do rational functions above`

`that's probably it for this section`



