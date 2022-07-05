TEXT: A Transition to Advanced Mathematics

$\textsection~4.2$ Sequences

A #sequence is a function $x$ with a domain $\mathbb{N}$. 

__nth term of the sequence:__ given by $x_{1}, x_{2}, x_{3}..., \mathbf{x_{n}}$ 

For example, the sequence whose nth term is $x_{n}=\dfrac{(-1)^{n}}{n+1}$ illustrates the convergence property of sequences. 

The first few terms of x are as follows:

$$\begin{align*}
x_{1}=\frac{-1^{1}}{1+1}&=-\frac{1}{2}\\
x_{2}=\frac{-1^{2}}{2+1}&=\frac{1}{3}\\
x_{3}=\frac{-1^{3}}{3+1}&=-\frac{1}{4}\\
\vdots~~~~~~~~~~~~~~~~&\\
x_{99}= \ldots \ldots &=-\frac{1}{100}\\\\
\vdots~~~~~~~~~~~~~~~~&\\
x_{1000}= \ldots \ldots &=-\frac{1}{1001}\\
\end{align*}$$

The pattern shows that regardless of sign, x $\rightarrow$ 0 from both directions, that is, $\forall n \ge 0,~~~x \rightarrow 0$ 

__We say the__ #limit __of this sequence is 0__ 

This notion is made precise in the following definition:

$\mathbf{x_{n} \rightarrow L}$: For a sequence $x$ of real numbers and a real number L , we say that $x$ has the _limit L_ (or $x$ _converges_ to L) #convergent __if__ for every $\epsilon>0$ there exists a natural number N such that if $n>N$, then $|x_{n}-L| < \epsilon$. When x converges to the real number L, we write $\displaystyle{\lim_{n \to \infty} x_n =L}$ or $x \rightarrow L$. If no such number L exists, we say $x$ _diverges_ or $\displaystyle{\lim_{n \to \infty} x_n}$  _does not exist._ #divergent

_A takeaway from this definition is that it is usually assumed that_ $\epsilon$ _as being a small positive number, so the expression_ $|x_{n}-L| < \epsilon$ _means that the distance between_ $x_n$  _and L is small._  

__Epsilon-Delta Proof frame  that__ $\mathbf{\displaystyle{\lim_{n \to \infty} x_{n}=L}}$. 

Proof:

Let $\epsilon$ be a real number greater than 0 ($\epsilon >0$).

Choose $N =$ some number, usually in terms of $\epsilon$

Let $n \in \mathbb{N}$, and suppose that $n > N$ 

$\vdots$

Therefore, $|x_{n}-L| < \epsilon$.

We can conclude that $\displaystyle{\lim_{n \to \infty} x_{n}=L}$

_Another takeaway - in order to verify that_ $|x_{n}-L| < \epsilon$ , consider both $n$ and $\epsilon$ and find a relationship between them that will suggest a choice for N. With the original assumption that $n>N$, when a relationship between $\epsilon$ and $n$ is made, statements can also be made about $N$.



#### Example 1
Show that $x_{n}= \dfrac{(-1)^{n}}{n+1}$ converges and $\displaystyle{\lim_{n \to \infty} \frac{(-1)^{n}}{n+1}=0}$. 

_backwork_

_We Need To Show_ a relationship between $x_{n}$ and $\epsilon$ using $|x_n - 0| < \epsilon$. For any $\epsilon >0$, it follows that

$$|x_{n}-0|=|x_{n}|=\bigg|\frac{(-1)^{n}}{n+1}\bigg|=\frac{1}{n+1}$$
and so 
$$\frac{1}{n+1}< \epsilon.$$
With some algebra
$$
\begin{align*}
n+1\cdot\frac{1}{n+1}&< \epsilon\cdot n+1\\\\
1&<\epsilon(n+1)\\\\
\frac{1}{\epsilon}&<n+1\\\\
n+1&>\frac{1}{\epsilon}\\\\
n&>\frac{1}{\epsilon}-1
\end{align*}
$$
We can say that since $n>N$, let $N$ be any integer greater than $\dfrac{1}{\epsilon}-1$.

Proof:

Let $\epsilon$ be a positive real number. Let $N$ be any integer greater than $\dfrac{1}{\epsilon}-1$. Suppose that $n>N$. Then $n>\dfrac{1}{\epsilon} -1$, and with some algebra


Convergent vs Divergent

A sequence is said to be #convergent  if it's _limit_ exists. Else, it is said to be #divergent .

Also, if the limit is infinite, the sequence is also said to be divergent. 

Examples of Convergent Sequences

The sequence $\frac{1}{n}$ is convergent, because $\displaystyle{\lim_{n \to \infty} \frac{1}{n}=0}$

The constant sequence $c$ is convergent, with $c \in \mathbb{R}$ because $\displaystyle{\lim_{n \to \infty} c =c}$

The sequence $\big(1+\frac{1}{n}\big)^n$ is convergent, because $\displaystyle{\lim_{n \to \infty} \bigg(1+\frac{1}{n}\bigg)^n=e}$

Examples of Divergent Sequences

The sequence $n$ is divergent, because $\displaystyle{\lim_{n \to \infty} n=\infty}$ and the sequence $-n$ is divergent, because $\displaystyle{\lim_{n \to \infty} n=-\infty}$

The sequence $a_{n}=\dfrac{4x^{3}+5x}{3x^{2}+8}$ is divergent, because after utilizing L'Hospital's Rule to find the limit 

$$\displaystyle{\lim_{n \to \infty} \dfrac{4x^{3}+5x}{3x^{2}+8}} \rightarrow \lim_{n \to \infty} 4x=\infty$$
The sequence $(-1)^n$ is divergent, because $\displaystyle{\lim_{n \to \infty} (-1)^n=\text{DNE}}$ 