---
use_math: true
title: Product Rule
---

# Product Rule

Taking the derivative of a sum or difference of functions is straightforward and intuitive. We have that $(f+g)' = f' + g'$ and $(f-g)' = f' - g'$. We might then be tempted to think that the same idea applies to the product of functions: i.e. that $(fg)' = f'g'$.

But this is wrong!

As an example, if $f(x) = x^2$, then we know that $f'(x) = 2x$. But we can also write $f(x) = g(x)h(x)$ where $g(x)=h(x) =x$. Under the naive idea above, we'd have that $f'(x) = g'(x)h'(x) = 1$. So clearly this idea is wrong.

To explore this concept, it's helpful to think of the area of some rectangle given by the product of its length and width, both of which are varying in time.

$$
A(t) = l(t)w(t).
$$

After some small change in time $\Delta t$, the area of the rectangle is then

$$
A(t+\Delta t) = l(t+\Delta t)w(t+\Delta t).
$$

The change is area over $\Delta t$ is then given by

$$
A(t+\Delta t) - A(t) = l(t+\Delta t)w(t+\Delta t) - l(t)w(t).
$$

The right hand side can be thought of as the sum of three small rectangles: $(l(t+\Delta t) - l(t))w(t) + (w(t+\Delta t)-w(t))l(t) + (l(t+\Delta t)-l(t))(w(t+\Delta t)-w(t))$.

$$
A(t+\Delta t) - A(t) = (l(t+\Delta t) - l(t))w(t) + (w(t+\Delta t)-w(t))l(t) + (l(t+\Delta t)-l(t))(w(t+\Delta t)-w(t)).
$$

If we then divide both sides by $\Delta t$ and take the limit as $\Delta t$ goes to $0$, we get

$$
\lim_{\Delta t \rightarrow 0} \frac{A(t+\Delta t) - A(t)}{\Delta t} = \lim_{\Delta t \rightarrow 0}\frac{(l(t+\Delta t) - l(t))w(t) + (w(t+\Delta t)-w(t))l(t) + (l(t+\Delta t)-l(t))(w(t+\Delta t)-w(t))}{\Delta} = l'(t)w(t) + w'(t)l(t).
$$

Thus the product rule is:

>**Product Rule**
>
> $(fg)' = f'g + fg'$ wherever both $f$ and $g$ are differentiable.


## Quotient Rule

Given that if $A = lw$ we have $A' = l'w + lw'$, it's then true that $l' = (A' - lw')/w = (A' - Aw'/w)/w = (A'w - Aw')/w^2$. This means that $(A/w)' =  (A'w - Aw')/w^2$ since $l = A/w$. This is the quotient rule:

> **Quotient Rule**
>
> $\left( \frac{f}{g} \right)' = \frac{f'g - fg'}{g^2}$ wherever both $f$ and $g$ are differentiable.
