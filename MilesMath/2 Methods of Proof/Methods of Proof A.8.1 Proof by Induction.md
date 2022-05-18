[[Methods of Proof 0.0.0 Induction Proof]]

Prove by induction that for every $n=1,2,3...,$ $$1^2+2^2+3^2+...+n^2=\frac{n(n+1)(n+2)}{6}$$

Proof: 
Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 
BASIS STEP:
Let $n=1$ (To show that $P(n)$ is true) 
$$\begin{align}
P(n)&=\frac{n(n+1)(2n+1)}{6}\\
P(1)&=\frac{1(1+1)(2(1)+1)}{6}\stackrel{?}{=} 1^2\\
P(1)&=\frac{6}{6}=1=1^2~\checkmark
\end{align}$$
$\therefore P(1)$ is true and $1\in S$ so $S$ is not empty.

INDUCTION STEP: 
Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$
We know $P(k)=\frac{k(k+1)(2k+1)}{6}$, consider $n=k+1$.

Must show that 
$$
P(k)=\frac{k(k+1)(2k+1)}{6} \Rightarrow P(k+1)=\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6}
$$
Utilizing the induction hypothesis with $n=k+1$:
$n-1=k$, plugged into $P(k)$ gives: 
$$\begin{align*}
P(k)&=\frac{k(k+1)(2k+1)}{6}\\
P(n-1)&=\frac{(n-1)(n-1+1)(2(n-1)+1)}{6}\\
P(n-1)&=\frac{n(n-1)(2n-1)}{6}\\
\end{align*}$$
since $n=k+1$

$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 
(To show that whatever statement is true for any positive integer $m$, show it is also true for the next integer $m+1$)




Back work



So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

---
