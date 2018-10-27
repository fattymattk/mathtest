---
use_math: true
title: Derivatives
---

# Derivatives

The slope of the line can be thought of as "rise over run", i.e. a vertical change divided by a horizontal change. Given two points $(x_1,y_1)$ and $(x_2,y_2)$ on a line, we define the slope $m$ to be:

$$
m = \frac{y_2 - y_1}{x_2 - x_1}.
$$

This of course can be negative, in which case we can picture the graph of the line going down to the right. If the slope is positive, the line goes up to the left, and if it's zero, the line is perfectly horizontal.

The slope of the line tells us its **rate of change**. If we have position on the vertical axis and time on the horizontal axis, then the slope of a line tells us a speed. For example, we might have the position $x$ of a car at time $t$ given by

$$
x(t) = 3t + 1.
$$

At $t=1$, the position of the car is $x(1) = 3(1) + 1 = 4$, and at $t=2$, the position of the car is $x(2) = 3(2) + 1 = 7$. The change is position from $t=1$ to $t=2$ is then $7-4=3$. So we can say the car went $3$ units of distance in $1$ unit of time. Intuitively, we should then think the speed of the car is $3$ distance units per time unit. This is exactly the slope of the line:

$$
m = \frac{x(2)-x(1)}{2-1} = \frac{7-4}{2-1} = 3.
$$

When $x(t) = 3t + 1$, the car is always traveling at a constant velocity of $3$, and we can see this by observing that the graph is a straight line. But we know in reality that cars are able to speed up and slow down, so their velocity can change. With a non-constant velocity, the graph of position versus time should look like a curve.

The question then is: if a car is changing its speed as time moves on, how can we define its velocity at some given time? The graph won't be a straight line, so we simply can't take two points on the graph and measure the rise over run. But we might except we want to do something similar to this, and that the graph of a curve might still have some well-defined "steepness" to it at a given point.

This "steepness" at a given point can be defined to be the slope of the **tangent line** to the curve at the given point. A tangent line can be thought of as the line that best approximates the curve at the point. It is positive if the tangent line goes up to the right, negative if the it goes down to the right, or $0$ if it is perfectly horizontal.

While we actually need two points on the graph to define a rise and a run, we can still determine a slope at a single point. Say we want to determine the slope at point $a$. We consider the rise over run of a line connecting $(a,f(a))$ and $(x,f(x))$ and then let $x$ approach $x$. This is given by

$$
\lim_{x \rightarrow a} \frac{f(x)-f(a)}{x-a}.
$$

This is in fact the definition of the **derivative** of $f$ at $a$. We denote this as $f'(a)$. We then have the definition of the derivative:

$$
f'(a) = \lim_{x \rightarrow a} \frac{f(x)-f(a)}{x-a}.
$$

Note that this limit might not exist. In that case we say that the derivative of $f$ at $a$ doesn't exist, or that $f$ is not differentiable at $a$. For example, if the graph of $f(x)$ has a sharp corner at $a$, we don't expect there to be a well-defined tangent line there, and so $f'(a)$ wouldn't exist in that case.




