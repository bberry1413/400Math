The sequence is defined recursively by 

$$f_{1}=1,~~f_{2}=1,~~f_{n+2}=f_{n}+f_{n+1}$$

is called the _Fibonacci sequence_. It is possible to find an explicit formula for this sequence. 

1, 1, 2, 3, 5, 8, 13, 21, 34, 55...

$f(x)=x+b$ for arithmetic progressions

$f(x)=ax$ for geometric progressions

$$\begin{align*}
x_{1}&=1\\
x_{2}&=1\\
x_{3}&=2\\
x_{4}&=3\\
x_{5}&=5\\
x_{6}&=8
\end{align*}$$


$f_{n}=\dfrac{1}{\sqrt{5}}\Bigg\{\Big(\dfrac{1+\sqrt{5}}{2}\Big)^{n}-\Big(\dfrac{1-\sqrt{5}}{2}\Big)^{n}\Bigg\}$ 

verify through induction

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true

**BASIS STEP:** Let $n=1$ *(To show that* $P(n)$ *is true)* 

$f_{1}=\dfrac{1}{\sqrt{5}}\Bigg\{\Big(\dfrac{1+\sqrt{5}}{2}\Big)^{1}-\Big(\dfrac{1-\sqrt{5}}{2}\Big)^{1}\Bigg\}=\frac{1}{\sqrt{5}}\Big(\sqrt{5}\Big)=1$

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$

*We Need To Show:* $P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align*}
P(k)&=\dfrac{1}{\sqrt{5}}\Bigg\{\Big(\dfrac{1+\sqrt{5}}{2}\Big)^{k}-\Big(\dfrac{1-\sqrt{5}}{2}\Big)^{k}\Bigg\}\\
P(k+1)&=\dfrac{1}{\sqrt{5}}\Bigg\{\Big(\dfrac{1+\sqrt{5}}{2}\Big)^{k+1}-\Big(\dfrac{1-\sqrt{5}}{2}\Big)^{k+1}\Bigg\}\\
\end{align*}$$

With some algebra, $P(k+1)$ can be rewritten as:

$$\begin{align*}
P(k+1)&=\dfrac{1}{\sqrt{5}}\Bigg\{\Big(\dfrac{1+\sqrt{5}}{2}\Big)^{k+1}-\Big(\dfrac{1-\sqrt{5}}{2}\Big)^{k+1}\Bigg\}\\
&=\dfrac{1}{\sqrt{5}}\Bigg\{\Big(\dfrac{1+\sqrt{5}}{2}\Big)^{k} \cdot \Big(\dfrac{1+\sqrt{5}}{2}\Big) -\Big(\dfrac{1-\sqrt{5}}{2}\Big)^{k} \cdot \Big(\dfrac{1-\sqrt{5}}{2}\Big)\Bigg\}\\
&
&
\end{align*}$$


So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.