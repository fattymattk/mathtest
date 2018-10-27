---
use_math: true
title: Derivatives
---

# The Derivative as a Function

We've seen the definition of the derivative at a point of the function:

$$
f'(a) = \lim_{x \rightarrow a} \frac{f(x)-f(a)}{x-a}.
$$

Here, $a$ is interpreted as some fixed constant in the domain of $f$, and $f'(a)$ is the slope of the tangent line to the graph at $a$ (when it exists).

We can instead consider point where we're finding the derivative to be a variable. That is, we can interpret the definition to work for all possible points at once. In this case, we can consider the **derivative as a function**, which we denote by $f'$. This is a function that takes in real numbers, and outputs other real numbers. We define the function by

$$
f'(x) = \lim_{h \rightarrow 0} \frac{f(x+h)-f(x)}{h},
$$

and the domain of this function is wherever this limit exists.

For example, consider $f: \mathbb{R} \rightarrow \mathbb{R}$ defined by $f(x) = x^3$. Then $f'$ is defined by

$$
f'(x) = \lim_{h \rightarrow 0} \frac{(x+h)^3-x^3}{h}.
$$

Expanding the numerator out, simplifying, and taking the limit, we get that

$$
f'(x) = 3x^2.
$$

This limit exists for any $x \in \mathbb{R}$, so we have that $f': \mathbb{R} \rightarrow \mathbb{R}$. That is at any point on the graph $(x,x^3)$, we have the slope of the tangent line there given by $3x^2$.

As another example, consider the function $g$ given by $g(x) = \frac{1}{x}$. The domain of $g$ is every real number except $0$. To find $g'$, we compute

$$
g'(x) = \lim_{h \rightarrow 0} \frac{\frac{1}{x+h}-\frac{1}{x}}{h}.
$$

Show that $g'(x) = \frac{-1}{x^2}$. What is the domain of $g'$?

> Theorem:
>
> If $f$ is differentiable at $a$ (i.e. if $f'(a)$ exists), then $f$ is continuous at $a$.

To prove this, we'll consider what's needed in order for $f'(a)$ to exist. We have that

$$
f'(a) = \lim{x \rightarrow a} \frac{f(x)-f(a)}{x-a}
$$

exists. The first thing to notice is that this definition requires that $f(a)$ is defined. So $f$ cannot be differentiable at $a$ if $a$ is not in the domain of $f$. We then want to show that 

$$
\lim_{x \rightarrow a} f(x) = f(a).
$$

We have that 

$$
\lim_{x \rightarrow a} f(x) = f(a) - f(a) + \lim_{x \rightarrow a} f(x) = f(a) + \lim_{x \rightarrow a} \[f(x) - f(a)\]= f(a) + \lim_{x \rightarrow a} (x-a)\frac{f(x) - f(a)}{x-a} = f(a) + \lim_{x \rightarrow a} (x-a) \lim_{x \rightarrow a} \frac{f(x) - f(a)}{x-a} = f(a) + 0 \cdot f'(a) = f(a).
$$

This should seem intuitive if we think of the graph of $y=f(x)$. If $f$ is not continuous at a point, it seems hard to imagine that we are able to construct a tangent line there.

We can therefore conclude that the domain of $f'$ is a subset of the set of points where $f$ is continuous.

It's important to note that the converse of the above result is not true. That is, if a function is continuous at a point, that **does not** imply that the function is differentiable there. As an example, consider the function $h: \mathbb{R} \rightarrow \mathbb{R}$ defined by $h(x) = |x|$.

Let's see if $h$ is continuous at $0$. We have that $h(0) = |0| = 0$. We have that 

$$
\lim_{x \rightarrow 0^+} h(x) = \lim_{x \rightarrow 0^+} x = 0,  
$$

and

$$
\lim_{x \rightarrow 0^-} h(x) = \lim_{x \rightarrow 0^-} -x = 0.  
$$

Therefore

$$
\lim_{x \rightarrow 0} h(x) = 0,  
$$

so $h$ is continuous at $0$. 

To see if it's differentiable, consider

$$
\lim_{k \rightarrow 0} \frac{h(0+k)-h(0)}{k}.
$$

From the right, we have 

$$
\lim_{k \rightarrow 0^+} \frac{h(0+k)-h(0)}{k} = \lim_{k \rightarrow 0^+} \frac{k-0}{k} = 1.
$$

From the left, we have 

$$
\lim_{k \rightarrow 0^-} \frac{h(0+k)-h(0)}{k} = \lim_{k \rightarrow 0^-} \frac{-k-0}{k} = -1.
$$

To the limit doesn't exist. This means $h'(0)$ doesn't exist and we can say that $h$ is not differentiable at $0$, even though it's continuous there.




