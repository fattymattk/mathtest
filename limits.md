---
use_math: true
title: Limits
---

# Limits

The idea of the limit is perhaps the most important concept in Calculus. It's a perhaps subtle idea that might take some getting use to. It's a concept that needs to be understood well.

Let's take a look at the function $f$, defined by

$$ f(x) = \frac{x^2-9}{x-3}.$$

The graph can be found [here](https://www.desmos.com/calculator/cjhohrcelo).

If we slide the $a$ slider so that $a=2$, we can see what $f(a)$ is at that input: $f(a) = 5$. Of course, we could also determine this just by evaluating the function: $f(2) = \frac{2^2-9}{2-3} = \frac{4-9}{-1} = \frac{-5}{-1} =5.$

Similarly, we can determine $f(a)$ for a varierty of values of $a$, say $a=3.2$ for example.

However, something happens when we move the $a$ slider to $a=3$. Desmos tells us that $f(a)$ is undefined. Well of course it is! The denominator of $\frac{x^2-9}{x-3}$ is $0$ when $x=3$, and we are not allowed to divide by $0$. Simply put, $3$ is not in the domain of $f$.

However, the graph suggests that even though we can't use $3$ as an input, there's still something to be said about inputs that are *close* to $3$. For example, if we look at $a=2.9$, we get that $f(a)=5.9$. If we look at $a=3.1$, we get that $f(a) = 6.1$. So it appears that if we're hanging out in the neighbourhood of $a=3$ without being exactly at $a=3$, we're somehow in the neighbourhood of $f(a)=6$.

What happens if we get closer? If $a=2.999$, $f(a) = 5.999$ and if $a=3.001$, $f(a)=6.0001$. So by making $a$ closer to $3$, but not equal to $3$, we see that $f(a)$ gets closer to $6$.

Is it possible to see why this is happening? Let's try manipulating what the function looks like.

Using difference of squares, we can rewrite the function as

$$f(x) = \frac{(x-3)(x+3)}{x-3}.$$

If we're careful to point out that $x\neq 3$, then we can divide the numerator and denominator by the factor $(x-3)$. This yields:

$$f(x) = x+3, \hspace{1cm} \mbox{for } x \neq 3.$$

So we have confirmed our above observations: as long as out input $a$ is not equal to $3$, the output is simply $f(a) = a+3$. And indeed, the closer $a$ gets to $3$, the closer $f(a)$ gets to $3+3=6$.

As another example, consider the function $g$ defined by:

$$g(x) = \frac{|x-3|}{x-3}.$$

The graph of which can be found [here](https://www.desmos.com/calculator/n39so7nnvd).

Again, this function is not defined for $x=3$, since then we're dividing by $0$. However, looking at the graph, we see that something different is happening for input values close to $3$. If $a<3$, then $f(a) = -1$, and if $a>3$, then $f(a) = 1$. So in this case it's not so simple to say that if $a$ is close to $3$, but not equal to $3$, then $f(a)$ is close to some value$. That is, if we're in the neighbourhood of $a=3$ we can't say what neighbourhood $f(a)$ is hanging out in.

This brings us to the concept of a limit. In words, we'll make the following definition:

`I have a big problem here using a as a variable input`

>Definition:
>
>Let $f:A \rightarrow B$ be a function. We say that the limit of $f$ at $a$ is equal to $L$, and write $\lim_{x \rightarrow a} f(x) =L$ if we can make $f(x)$ as close as we want to $L$ for all $x$ sufficiently close to, but not equal to, $a$.

Considering our example above where $f(x) = \frac{x^2-9}{x-3}$, we can consider the limit of $f$ at $3$. For $x\neq 3$, we have $f(x) = x+3$. We expected the limit to be $6$. Indeed, if we want $f(x)$ to be within $0.1$ of $6$, we just need to take $x$ within $0.1$ of $3$. If we wanted $f(x)$ to be within $0.0001$ of $6$, we just need to take $x$ within $0.0001$ of $3$. 

However, for $g(x) = \frac{|x-3|}{x-3}$, the limit of $g$ at $3$ does not exist. That's because $g(x)$ does not get close to any single value $L$ when $x$ is near $3$. If we were to suppose that the limit is $1$, then we would require all $x$ inputs that are close to $3$ but not equal to $3$ to give outputs close to $1$. But inputs slightly less than $3$ give outputs of $-1$. So there's no way to guarantee that $f(x)$ can be made as close to $1$ as we want by requiring that $x$ be close enough to $3$. Indeed, any neighbourhood around $3$ will include inputs less than $3$, which output $-1$, which isn't close to $1$.

## Numerical Evidence of a Limit

Without having any tricks in order to evaluate a limit, we can proceed somewhat naively and use what we know from the definition to try and guess a sensible value of what a limit might be. 

Consider the function $f$ defined as the following:

$$ f(x) = \frac{x^2 + 1}{x-2}.$$

As a side note, the domain of this function is all real numbers except $x=2$. The codomain can be taken to be $\mathbb{R}$ and the range is some subset of $\mathbb{R}$ that we don't really care about right now.

Suppose we want to evaluate the following:

$$\lim_{x\rightarrow 1} f(x).$$

We can't just evaluate $f(1)$ because the definition of the limit tells us we're interesting in $f(x)$ for $x$ close to $1$, *but not equal to $1$*. Given this, the natural thing to do is to try out different values of $x$ that get closer and closer to $1$ and see what happens.

We take a look at the graph [here](https://www.desmos.com/calculator/pywkn1cgxa) and move the value of $a$ around to see what happens when $a$ gets close to $1$. 

|   a           |  f(a)             | 
| ------------- |:-----------------:| 
| 0.9           | -1.645454545...   |
| 0.99          | -1.9604950495...  |
| 0.999         | -1.996004995...   |


So we have numerical evidence that when $a$ is close to $1$, but less than $1$, $f(a)$ is close to $-2$. Furthermore, the closer we get to $1$, the closer we get to $-2$. So $-2$ seems like a good candidate for our limit. But this isn't quite enough evidence yet, as we should investigate what happens what happens on the other side of $1$ (we could get some weird behaviour like for $g$ above).

|   a           |  f(a)             | 
| ------------- |:-----------------:| 
| 1.1           | -2.455555555...   |
| 1.01          | -2.04050505051... |
| 1.001         | -2.00400500501... |

And indeed, when $a$ is close to $1$, but greater than $1$, $f(a) is close to $-2$. So it seems like 

$$\lim_{x\rightarrow 1} \frac{x^2+1}{x-2} = -2.$$

Now note that this is not proof. We will learn some tricks to evaluate limits more carefully, rather than relying on this tedious and perhaps unreliable numerical method. We just do this now to get a feeling for what a limit is. In a sense, it's the value of a function at some input if we're not allowed to use the input.

Also note that if we take a look at the graph of $y=f(x)$ in our current example, it's kind of obvious what the limit is. The limit is clearly $f(1)$. So why can't we just evaluate $f(1)$ and say that that's the limit?

There are two reasons: (1) We're not always able to evaluate the function at the input we're interested in, as it's not always in the domain of the function, and (2) The limit is not always the same as the value of the function at that input.

To expand on the second reason, consider the piecewise function $h$, defined by

$$ h(x) = \left\{ \begin{array}{ll} x^2, & \mbox{if } x < 0, \\ x+1, & \mbox{if } x \geq 0. \end{array} \right.$$
