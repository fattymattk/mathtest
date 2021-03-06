---
use_math: true
title: Numbers
---


# Numbers

It might seem silly to talk about what numbers are. We've been dealing with them since we were children, and we have a pretty good idea of what they are.

But just to make sure we're all speaking the same language, let's make some definitions.

>Definition:
>
>The **natural numbers**, denoted by $\mathbb{N}$, are simply the "counting" numbers: $0,1,2,3,4,5,...$ and so on.

Note that it's not uncommon to exnclude $0$ in the definition. Don't worry too much about this, either definition is okay as long as one is clear about what they mean.

We can add any two natural numbers together and get back another natural number. For example, if we add $5$ to $3$, we get $3+5=8$, and $8$ is also a natural number. We can also multiply any two natural numbers together and get back another natural number: $7\cdot6 = 42$, and $42$ is a perfectly acceptable natural number.

However, it's not true that we can always subtract a natural number from another to get back another natural numbers. If we subtract $5$ from $3$, we get... well, we actually can't do that! But that brings us to our next number system.

>Definition:
>
>The **integers**, denoted by $\mathbb{Z}$, are the natural numbers and their negative values: $...-3,-2,-1,0,1,2,3,...$.

The integers also have the property that we can add or multiply any two together and get back another. But the integers also have the property that we can subtract any integer from another, and get back another integer. For example, if we subtract $5$ from $3$, we get $3-5=-2$.

What we can't do though, is divide any two integers and get back another integer. Sometimes we can: for example, $6$ divided by $3$ is $6/3 =2$. But in general, we're not guaranteed another integer: within the integers, we cannot divide $5$ by $3$, for example, since $5/3$ is not an integer.

>Definition:
>
>The **rationals**, denoted by $\mathbb{Q}$, are the numbers that can be written in the form $p/q$, where $p$ and $q$ are integers, and $q\neq 0$.

There are many ways to write a given rational number. For example, $2$ is the same as $2/1$, which is the same as $6/3$ or $(-34)/(-17)$. So $p$ and $q$ in the definition are not unique.

It is also true that rational numbers have decimal expansions that either terminate or repeat. $1/3 = 1.33333...$, which repeats. $3/4 = 0.75$, which terminates. $2/7 = 0.285714285714285714...$, which has $6$ digits in the repeating pattern.

Of course, we can add, multiply, and subtract any two rationals and get back another. But what about division? The answer is yes, provided that what we are dividing by isn't $0$. We can never divide by $0$!


Let's remind ourselves how to divide a rational number by another.

Let $a=p/q$ and $b=s/t$, where $p,q,s$, and $t$ are integers, and $q,s$, and $t$ are not equal to $0$. Then $a$ divided by $b$ is:

$$
\begin{align*}
\frac{a}{b} &= \frac{\frac{p}{q}}{\frac{s}{t}}, \\
&= \frac{p}{q} \cdot \frac{t}{s},\\
&= \frac{pt}{qs}.
\end{align*}
$$

Note that if $q$ or $t$ were $0$, then $a$ or $b$ would be undefined. If $s$ was $0$, then $b=0$, and $a/b$ would be undefined. 

Our next number system, which will be our final one, and the one we use most often in calculus, is a little harder to define. Let's reveal to ourselves its name: the **real numbers**. 

Roughly, the real numbers include the rational numbers and all the numbers in between them. This statement suggests there are numbers that aren't rational. 

An example of a number that isn't rational is $\sqrt{2}$. This number cannot be written in the form $p/q$ where $p$ and $q$ are integers, and if we were to write out its decimal expansion, it would never terminate or repeat. We call real numbers that are not rational **irrational**.

>Definition:
>
>The **real numbers**, denoted by $\mathbb{R}$, are the rational numbers and the irrational numbers.

The rational and irrational numbers together complete the numbers we're interested in. We won't go into detail about what this means, but briefly it means that given a real number $r$, all other real numbers are either less than $r$ or greater than $r$. The usual picture is that of a number line, and every real number has its place on it.


## Properties of the Real Numbers

We'll take the following properties to be true.

Given real numbers $a,b,$ and $c$, we have that:

1. $a+(b+c) = (a+b)+c$ (associativity of addition).

2. $a + 0 = a$.

3. $a+(-a) = 0$.

4. $a+b = b+a$ (commutativity of addition).

5. $a\cdot (b \cdot c) = (a\cdot b) \cdot c$ (associativity of multiplication).

6. $a\cdot 1 = a$.

7. If $a \neq 0$, then $a\cdot \frac{1}{a} = 1$.

8. $a\cdot b = b \cdot a$ (commutativity of multiplication).

9. $a\cdot (b+c) = a \cdot b + a \cdot c$ (distributivity).

Associativity doesn't need to much explaining. It's very natural, and it would be very unintuitive to work with a number system that wasn't associative. 

The number $0$ is called the **additive identity**. When doing addition, it's the number that keeps the other number the same. We call $-a$ the **additive inverse** of $a$. It's unique, so there's only one number we can add to $a$ to get $0$. We also have that $-(-a) = a$, which means the additive inverse of the additive inverse of $a$ is the same as $a$.

Commutativity is another intuitive property. It says that it doesn't matter which order we add numbers in, so we're free to change the order around if it suits us.

The number $1$ is called the **multiplicative identity**. When doing multiplication, it's the number that keeps the other number the same. We call $1/a$ the **multiplicative inverse** of $a$. Every number except $0$ has a multiplicative inverse, and it's unique. We also have that $\frac{1}{\frac{1}{a}} = a$. i.e. The multiplicative inverse of the multiplicative inverse of $a$ is the same as $a$.

The distributive property is also very natural, but we shouldn't take it for granted. Later, we might get into trouble if we try to apply it to situations that are inappropriate. 


##Ordering the Real Numbers

We use the symbol $<$ to mean "less than" and the symbol $>$ to mean "greater than". Hence, if we write $a<b$, then $a$ is less than $b$, which means that $a$ is farther left on the number line than $b$ is. 

We write $\leq$ and $\geq$ to respectively mean "less than or equal to" and "greater than or equal to." So $a\geq b$ means that either $a$ is greater than $b$ ($a$ is farther right on the number line than $b$ is) or $a$ is equal to $b$.

If $a>0$, we say that $a$ is **positive**. If $a<0$, we say that $a$ is **negative.**

Any real number is positive, negative, or 0. It cannot be two of these, and it also can't be none of these.

If $a\geq 0$, we say that $a$ is **nonnegative**. If $a\leq 0$, we say that $a$ is **nonpositive**. The only number that is both nonnegative and nonpositive is $0$.

We have the following properties to add to our list.

Given real numbers $a,b$, and $c$, we have that:

10. If $a>b$, then$a+c>b+c$.

11. If $a>b$ and $c>0$, then $a\cdot c>b\cdot c$. 

12. If $a>b$ and $c<0$, then $a\cdot c < b \cdot c$.


