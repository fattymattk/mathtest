---
use_math: true
title: Precise Definition of a Limit
---

# Precise Definition of a Limit

We saw previously that the limit of the function $f$ at $a$ is equal to $L$ if we can make $f(x)$ as close as we want to $L$ by requiring that $x$ be sufficiently close to, but not equal to, $a$. We now formalize this idea with the following precise definition:

>Definition:
>
>Let $f:A \rightarrow B$ be a function. We say that the limit of $f$ at $a$ is equal to $L$, and write $\lim_{x \rightarrow a} f(x) =L$ if for any $\epsilon > 0$, there exists $\delta > 0$ such that $|f(x)-L|< \epsilon$ whenever $0<|x-a|<\delta$.

In general, $\delta$ will depend on $\epsilon$.

The value of $\epsilon$ represents how close we want $f(x)$ to be to $L$. The value of $\delta$ represents how close we require $x$ to be to $a$ to ensure this happens.

It's common to think of this idea like a game. First, I tell you how close $f(x)$ needs to be to $L$, i.e. I give you a value of $\epsilon$. Then you win the game by finding a $\delta$ so that I am unable to find $x$ such that $0<|x-a|<\delta$ and $|f(x)-L|<\epsilon$.

For example, let's consider the function $f: \mathbb{R} \rightarrow \mathbb{R}$ defined by $f(x) = 2x + 3$. We want to show that
$$
\lim_{x\rightarrow 1} f(x) = 5.
$$

Using the notation from the above definition, we have $a=1$ and $L=5$.

Now let us go through a few steps in our "game." I'm going to tell you that $\epsilon = 0.1$, and your job is now to find $\delta$ such that $|f(x)-5| < \epsilon$ whenever $0<|x-1|<\delta$. That is, the distance from $f(x)$ to $5$ is less than $0.1$ if $x$ is close enough to $1$.

You'd first consider $\delta$ unknown and to be determined. Then make the assumption that $0<|x-1|<\delta$. Then you want to play around with this inequality until you're able to choose $\delta$ so that $|f(x)-5| < 0.1$. Note that $|f(x)-5| = |2x+3-5| = |2x-2| = 2|x-1|$. So, given that $0<|x-1|<\delta$, you can multiply each side of the inequality by $2$, and say that $0<2|x-1|<2\delta$. If you then choose $\delta$ such that $0.1=2\delta$, then you'll have what you need.






