---
use_math: true
title: Distance
---


# Distance

## Distance on the Real Line

If we take a look at the real line, then we should have a clear intuitive idea of what the distance between two numbers are. Roughly, it's how far away they are from each other. We expect certain things to be true, like the distance between $1$ and $3$ to be the same as the distance between $2$ and $4$. We'd also expect that a distance between two numbers can't be negative, and that the distance from a number to itself should be $0$. 

We'll take the following definition to be our formal notion of distance:

>Definition:
>
> Let $a$ and $b$ be real numbers. The **distance** between $a$ and $b$ is $b-a$ if $b> a$ and $a-b$ if $a > b$ and $0$ if $a=b$. We denote the distance between $a$ and $b$ as $\|a-b\|$.

So to find the distance between two numbers, we take the bigger one and subtract the smaller one from it. The distance between $2$ and $1$ is therefore $2-1$, which is $1$. The distance between $-2$ and $37$ is $37-(-2)$, which is $39$.

Note that the distance between $x$ and $x$ is $x-x$, which is $0$. So if neither number is bigger than the other, then they're the same number, and so the distance is $0$. 

It should also be clear that if $a$ and $b$ are not the same number, then the distance between them is positive.

It should also be clear that the distance between $a$ and $b$ is the same as the distance between $b$ and $a$. So $|a-b| = |b-a|$.

The last property, which might not be obvious at first, is that $|a-c| \leq |a-b| + |b-c|$ for any real numbers $a,b$, and $c$. We call this the **triangle inequality**. You can think of it as going from $a$ to $c$ can't be farther the going from $a$ to $b$ and then from $b$ to $c$. If $b$ is between $a$ and $c$, then each trip should be the same either way. Otherwise, you're going out of your way to include $b$ on the journey.

