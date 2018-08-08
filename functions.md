---
use_math: true
title: Functions
---

# Functions

Roughly speaking, a function is a thing that takes an element of a set and maps it to an element in a different set. We write $f: A \rightarrow B$ to mean the following:

$f$ is a function that maps elements in set $A$ to elements in set $B$. If $x$ is in $A$, then we can think of $x$ as an input for the function. We write $f(x)$ to be the output of the function $f$ when the input is $x$. If $y=f(x)$ for some $x$ in $A$, then we require $y$ to be in set $B$.

We call $A$ the **domain** of $f$. We call $B$ the **codomain** of $f$.

We will only be interested in functions that have real numbers as inputs and outputs. Hence, $A$ and $B$ will always be subsets of $\mathbb{R}$.

> **Definition:**
>
>A **function** $f: A \rightarrow B$ is a rule that assigns to each element $x \in A$ exactly one element in $B$. This element in $B$ is denoted by $f(x)$ and is the **value** of $f$ at $x$.

We should note that "exactly one element" means that an input $x$ cannot have two different output values. That is, if $f(x) = y$ and $f(x) = z$, then $y = z$. For this reason, there is never any ambiguity by what we mean by $f(x)$. It only has one value!

It's unfortunately common to refer to $f(x)$ as a function. While we have no choice but to excuse such behaviour, we can still point it out as incorrect. $f$ is a function. $f(x)$ is the value of the function when the input is $x$. Simply put, $f$ is a rule or a formula, and $f(x)$ is a number. These are very different things! Just like a recipe is different than the meal it produces, a function is different than the numbers it outputs.

## Equations

An equation is just a statement expressing the equality of two values. Often it involves two variables, such as $x$ and $y$. In many cases, it's understood that one of the variables is to be thought of as the **dependent** variable while the other is to be thought of as the **independent** variable. The independent variable can be thought of as something we know and so therefore an input. The dependent variable can then be thought of as something we wish to determine, and therefore an output.

As an example, consider the following equation:

$$ y = x^2.$$

If we think of $y$ as the dependent variable and $x$ as the independent variable, then we can determine what $y$ is for a given value of $x$. For instance, if $x = 3$, then $y = 3^2$. We then know that $y = 9$ when $x = 3$.

On the other hand, if we consider $x$ to be the dependent variable and $y$ to be the independent variable, then things don't work out quite as nicely. If we are given that $y=9$, then it's not clear what $x$ should be$. If $x=3$ then the equation is satisfied, and if $x=-3$ then the equation is also satisfied.

If the equation is such that there is a unique value for the dependent variable for every value of the independent variable, then we can say that the dependent variable is a function of the independent variable. In our current example, we can say that $y$ is a function of $x$. That is, we can define a function $f$ such that $y=f(x)$. Here, $f$ is the function that maps a real number to its squared value.

However, we cannot say that $x$ is a function of $y$. If we try to define a function $g$ such that $x=g(y)$, then we run into problems since there are values of $y$ (say, $y=9$) that correspond to two values of $x$ ($x=3$ and $x=-3$).

## Graphs

Given an equation that relates variables $x$ and $y$, we can create a graph as the set of all pairs $(x,y)$ that satisfy the equation. Typically we put the dependent variable on the vertical axis and the independent variable on the horizontal axis. Then, for instance, the point $(1,2)$ is shown as the point $1$ unit right of the origin, and $2$ units up from the origin. The point $(-1,-2)$ would be shown $1$ unit left of the origin and $2$ units down from the origin.

In Desmos, this is done simply by typing in the equation. The convention is that $y$ is used for the dependent variable and $x$ is used for the independent variable. So for instance, if we type in `y=x^2`, we get the following graph:

![Graph of $y=x^2$](images/testgraph.png, "Graph of y=x^2").

The graph can be found [here](https://www.desmos.com/calculator/cgwhdkpkdt).

We can see that the points $(3,9)$ and $(-3,9)$ are points on the graph, as they satisfy the equation.

## Vertical Line Test






