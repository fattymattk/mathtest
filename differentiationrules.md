---
use_math: true
title: Differentiation Properties
---

# Differentiation Properties

Here we'll look at some useful properties of the derivative.

## Derivative of a Constant Function

Recall the $f$ is a constant function if there is a real number $c$ such that $f(x) = c$ for all $x$. The graph of this $y=f(x)$ is just a horizontal line at $y=c$. Hence, we should expect that the slope of the tangent line is $0$ for all $x$ values. Indeed:

$$
f'(x) =\lim_{h \rightarrow 0} \frac{f(x+h)-f(x)}{h} = \lim_{h \rightarrow 0} \frac{c-c}{h} = \lim_{h \rightarrow 0} 0 = 0.
$$

Therefore, **the derivative of a constant is $0$.**

## Derivative of a Constant Multiplied by a Function

If we define $g$ such that $g(x) = cf(x)$ for some real $c$, and take the domain of $g$ to be the domain of $f$, then $g'(x) = cf'(x)$ wherever $f'(x)$ exists. This is because:

$$
g'(x) = \lim_{h \rightarrow 0} \frac{g(x+h)-g(x)}{h} =\lim_{h \rightarrow 0} \frac{cf(x+h)-cf(x)}{h} =c\lim_{h \rightarrow 0} \frac{f(x+h)-f(x)}{h} = cf'(x).
$$

So we can pull constants out of the differentiation process. For example, if $g(x) = 3 x^2$ and $f(x) = x^2$, then $g'(x) = 3 f'(x) = 3 (2x) = 6x$.

We can just think of this as ``$3$ multiplied by the derivative of $x^2$.''

## Sum/Difference of Two Functions

Given two functions $f$ and $g$, if $f'(x)$ and $g'(x)$ both exist, then $(f+g)'(x) = f'(x) + g'(x)$ and $(f-g)'(x) = f'(x) - g'(x)$.

Because

$$
(f+g)'(x) = \lim_{h \rightarrow 0} \frac{(f+g)(x+h) - (f+g)(x)}{h}= \lim_{h \rightarrow 0} \frac{f(x+h)+g(x+h) - f(x) - g(x)}{h}= \lim_{h \rightarrow 0} \frac{f(x+h) - f(x)}{h}+\lim_{h \rightarrow 0} \frac{g(x+h) - g(x)}{h} = f'(x) + g'(x),
$$

since both limits exist. The proof for the difference is similar enough.

With the power rule and these properties of the derivative, we are now prepared to differentiate any polynomial. For example, if $p(x) = 4x^2 + 5x - 8$, then 

$$
p'(x) = (4x^2 + 5x - 8$)' = (4x^2)' + (5x)' - (8)' = 4(x^2)' + 5(x)' - (8)' = 4(2x^1) + 5(1x^0) - 0 = 8x + 5.
$$

Indeed, the sum/difference rule means we can differentiate each term one by one. The power rule and constant multiplier rules mean we can multiply the exponent of each term by the coefficient of the term, and then reduce the exponent by $1$. Finally, the constant rule means that constants just vanish under the derivative. 

So polynomials can be differentiated almost instantly. If $q(x) = 11x^7 - 3x^4 - 2x^2 + 10x + 34$, we have that $q'(x) = 77x^6 - 12x^3 - 4x + 10$.

