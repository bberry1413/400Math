TEXT: A Transition to Advanced Mathematics

$\textsection~4.2$ Sequences

A #sequence is a function $x$ with a domain $\mathbb{N}$. 

__nth term of the sequence:__ given by $x_{1}, x_{2}, x_{3}..., \mathbf{x_{n}}$ 

For example, the sequence whose nth term is $x_{n}=\frac{(-1)^{n}}{n+1}$ illustrates the convergence property of sequences. 

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

$\mathbf{x_{n} \rightarrow L}$: For a sequence $x$ of real numbers and a real number L , we say that $x$ has the _limit L_ (or $x$ #converges to L) __if__ for every $\epsilon>0$ there exists a natural number N such that if $n>N$, then $|x_{n}-L| < \epsilon$. When x converges to the real number L, we write $\displaystyle{\lim_{n \to \infty} x_n =L}$ or $x \rightarrow L$. If no such number L exists, we say $x$ #diverges or $\displaystyle{\lim_{n \to \infty} x_n}$  _does not exist._

_A takeaway from this definition is that it is usually assumed that_ \epsilon _as being a small positive number, so the expression_ $|x_{n}-L| < \epsilon$ _means that the distance between_ $x_n$  _and L is small._  

__Epsilon-Delta Proof frame  that__ $\mathbf{\displaystyle{\lim_{n \to \infty} x_{n}=L}}$. 

Proof:

Let $\epsilon$ be a real number greater than 0.

Choose N = some number, usually in terms of $\epsilon$

Let $n \in \mathbf{N}$, and suppose that $n > \mathbf{N}$ 

$\vdots$

Therefore, $|x_{n}-L| < \epsilon$.

We can conclude that $\displaystyle{\lim_{n \to \infty} x_{n}=L}$

_Another takeaway - in order to verify that_ $|x_{n}-L| < \epsilon$ , consider both n and \epsilon