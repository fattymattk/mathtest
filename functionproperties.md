---
use_math: true
title: Properties of Functions
---

# Properties of Functions

## Domain, Codomain and Range

In the previous section we defined a function $f: A \rightarrow B$ to be a mapping from the set $A$ to the set $B$. If $x \in A$, we call $x$ an input of the function, and we defined $f(x) \in B$ to be the corresponding output. We say that $A$ is the domain of the function $f$, and we require that each element of $A$ to have exactly one output. We call $B$ the codomain of the function $f$.

For example, if $f$ is the function that takes a number and returns its square root, then we can write $f(x) = \sqrt{x}$. Since we are not able to take the square root of negative numbers, a suitable domain for $f$ is the set $A=\\{x \in \mathbb{R} \| x\geq 0 \\}$. Since $\sqrt{x}$ is a real number for all $x\in A$, a suitable codomain is $B=\mathbb{R}$.

But that raises the question of whether or not there are elements in the codomain that have a corresponding output. The answer is *not necessarily*. We have that $-1$ is an element of $B$, but there is not $x\in A$ such that $\sqrt{x} = -1$.

This leads us to the concept of **range**. The range of a function is the set of all possible outputs. More precisely, the range is defined by $R=\\{y \in B \| f(x) = y \text{ for some } x\in A \\}$. It should be thought of as a subset of the codomain.

The difference between the codomain and the range of a function is perhaps a subtle one. The range is something the follows carefully and exactly from the definition of the function, while the codamin is a bit looser. All that's required of the codomain is that it contains the range. This can be convenient in cases where it's difficult or tedious to determine all the possible outputs of a function. Rather than going through that trouble, we can define the codomain to be something generous that we know contains all possible outputs, with the understanding that not every element in the codomain corresponds to an input.

So then if $f(x) = \sqrt{x}$, we can say that the range is $R=\\{x \in \mathbb{R} \| x\geq 0 \\}$. To see this, we get $y=f(x)$ and try to see which values of $y$ can be obtained. Squaring both sides of $y=\sqrt{x}$, we obtain $y^2 = x$ is neither $x$ or $y$ are negative. So indeed, if $y$ is any nonnegative number, plugging $y^2$ into $f$ gives us $f(y^2) = \sqrt{y^2} = |y| = y$. Since the square root of a number is never negative, we know thta $y$ cannot be negative. So indeed, $R$ is the range of $f$. While we took the codomain of $f$ to be $\mathbb{R}$, any set that contains $R$ would also be acceptable: say $\{y \in \mathbb{R} | y > -1 \}$ or even $R$ itself.

Given the graph of a function, we can determine the domain and range. The number $a$ is in the domain if and only if when we draw a vertical line at $x=a$, the line intersects the graph once (and only once). The number $b$ is in the range if and only if when we draw a horizontal line at $y=b$, the line intersects the graph at least once.

`We can do an example here, something like x/(x+1) for instance`

## Even and Odd Functions

>Definition:
>
>A function $f$ is called **even** if $f(x) = f(-x)$ for all $x$ in the domain of $f$. 
>
>A function $f$ is called **odd** if $f(x) = -f(-x)$ for all $x$ in the domain of $f$.

Thinking in terms of graphs, an even function is one where the $y$-axis acts in some way like a mirror. Put another way, if we had the graph printed on a piece of paper, and we folded the paper where the $y$-axis is, the graphs on either side of the $y$-axis would line up.

The following is a graph of an even function:

![Graph of Even Function](images/even_function.png "Graph of Even Function")

The graph can be found [here](https://www.desmos.com/calculator/muql8ewwkz).

Note the symmetry. The graph for positive $x$ values is the same for negative $x$ values, just reflected. We have, for example, $f(5) = f(-5)$ and $f(3) = f(-3)$, which agrees with the definition of what it means for a function to be even.



