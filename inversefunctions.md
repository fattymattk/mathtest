---
use_math: true
title: Inverse Functions
---


# Inverse Functions

## One-to-one Functions

>Definition:
>
>A function is called **one-to-one** if $f(x_1)=f(x_2)$ implies that $x_1=x_2$. Put another way, a function is one-to-one if $f(x_1)\neq f(x_2)$ whenever $x_1 \neq x_2$. 

Every output of a one-to-one function has a unique corresponding input. If $f$ is a one-to-one function, and I told you $a$ such that $f(x)=a$, you'd be able to tell me what $x$ is.

The classic example of a function that is **not** one-to-one, is the function $g: \mathbb{R} \rightarrow \mathbb{R}$ defined by $g(x)=x^2$. If I told you $g(x)=4$, you wouldn't be able to tell me what the input $x$ is. It could be that $x=2$, but it could be that $x=-2$. 

A simple example of a function that **is** one-to-one, is the function $h: \mathbb{R} \rightarrow \mathbb{R}$ defined by $h(x) = 2x-3$.
If I told you $h(x)=5$, you'd be able to tell me what $x$ is. You could set $2x-3=5$ and then solve for $x$. Adding $3$ to both sides, you'd get that $2x=8$. Dividing both sides by $2$, you'd get $x=4$. Since $x=4$ is the only solution, there is no question about what the input needed to be. More generally, if $h(x)=a$ where $a \in \mathbb{R}$, then $x=\frac{a+3}{2}$.

### The Horizontal Line Test

>A function $f$ is one-to-one if any horizontal line crosses the graph $y=f(x)$ at most one time. Otherwise, it is not one-to-one.

Indeed, if we look at the graph of $y=g(x)$, where $g(x)=x^2$, we can see that there are plenty of horizontal lines that cross the graph twice. Notably, corresponding to our above example, the horizontal line at $y=4$ crosses the graph at $(-2,4)$ and $(2,4)$.

For the example $h(x)=2x-3$, the graph $y=h(x)$ takes the form of a straight line. It's not hard to see that each horizontal line crosses the graph exactly once. As in our above example, the horizontal line at $y=5$ crosses the graph at $(4,5)$, and that's the only point of intersection. In the more general case, the horizontal line at $y=a$ crosses the graph at $((a+3)/2,a)$.

`need to do ordered pairs and graphs`

## The Domain is Important

Here's a question: if we define $f: [0,\infty) \rightarrow \mathbb{R}$ where $f(x) = x^2$, should we call $f$ a one-to-one function? The answer is yes. If $f(x) = a$ where $a$ is in the range of $f$, you could tell me what $x$ is. Set $x^2 = a$, and then square root both sides to get $x = \sqrt{a}$.  There is no longer any ambiguity, since the negative numbers are not part of the function's domain. Sketch the graph of this function and verify that it passes the horizontal line test.

For reasons such as this, the domain is an important part of a function's definition. Even though $f$ and $g$ have the same formula, their domains are different enough that they have very different properties.


## Inverse Functions

As a reminder, the **range** of a function is the set of all possible outputs. If $f: A \rightarrow \mathbb{R}$, then that's not enough to say that $\mathbb{R}$ is the range of $f$. All we can say is that the range is a subset of $\mathbb{R}$. 

>Definition:
>
> Let $f: A \rightarrow B$ be a one-to-one function. Let $C \subset B$ be the range of $f$. Then $f$ has what we call an **inverse function**, which we denote $f^{-1}$. The inverse function satisfies $f^{-1}: C \rightarrow A$ and $f^{-1}(f(x)) = x$ for all $x\in A$, and $f(f^{-1}(y)) = y$ for all $y \in C$. 


The inverse of $f$ maps the range of $f$ to the domain of $f$. So the domain of $f^{-1}$ is the range of $f$. It is also true that the range of $f^{-1}$ is the domain of $f$. 

The inverse is unique. A one-to-one function only has one inverse.

The inverse can be thought of as a way to undo a function. If we are given $a$ in the range of $f$, and we want to find $x$ such that $f(x)=a$, then the inverse gives us a way to do this. We apply the inverse function to both sides to get $f^{-1}(f(x)) = f^{-1}(a)$. By the above definition, the left hand side here is equal to $x$. So we get that $x=f^{-1}(a)$. This works for any $a$ in the range of $f$, since by definition the domain of $f^{-1}$ is the range of $f$. Since $f$ is one-to-one, we know there is a unique input for each output, so there is no ambiguity about what $f^{-1}(a)$ should be (it's a well-defined function).

As an example, let $f: [0,\infty) \rightarrow \mathbb{R}$ where $f(x) = x^2$. By the horizontal line test, we know $f$ is one-to-one. This means $f$ has an inverse that maps the range of $f$ to the domain of $f$. Let $y$ be in the range of $f$. Then $f(x)=y$ for some $x$ in the domain of $f$. This means $x^2=y$, which means $x = \sqrt{y}$ if $y\geq 0$. Therefore, the range of $f$ is $[0,\infty)$, since all outputs $y\in [0,\infty)$ have an input such that $f(x)=y$. We can then define $f^{-1}: [0,\infty) \rightarrow [0,\infty)$ by $f^{-1}(y) = \sqrt{y}$.

To verify that this is the inverse of $f$, let $x$ be in the domain of $f$. We then see that $f^{-1}(f(x)) = \sqrt{x^2} = x$. Now let $y$ be in the domain of $f^{-1}$. Then $f(f^{-1}(y)) = (\sqrt{y})^2 = y$. So this meets the definition of the inverse.

## The Graph of the Inverse Function

We can draw the graph $y=f^{-1}(x)$ by reflecting the graph of $y=f(x)$ about the line $y=x$.

This can also be thought of as switching the roles of $x$ and $y$. The graph $y=f(x)$ gives how the variable $y$ depends on the  variable $x$. By reflecting the graph about the line $y=x$, we are looking at how ther variable $x$ depends on the variable $y$. 

If you have trouble figuring out how such a reflection works, the following steps might be easier. Rotate the graph so that the positive $x$ axis points upwards and the positive $y$ axis points to the left. Then do a horizontal flip so that the positive $x$ axis is still pointing up, but the positive $y$ axis is now pointing to the right.

`an example graph would be great here`





