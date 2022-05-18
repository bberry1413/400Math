[[Methods of Proof 0.0.0 Induction Proof]]

Prove by induction that for every $n=1,2,3...,$ $$1^2+2^2+3^2+...+n^2=\frac{n(n+1)(2n+1)}{6}$$

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
Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$ and $k \ge 1$
 $$\begin{align}
 P(k)=1^{2}+2^{2}+3^{2} ...+(k-1)^{2} + k^{2}&=\frac{k(k+1)(2k+1)}{6}\\
 P(k+1)=1^{2}+2^{2}+3^{2} ...+((k+1)-1)^{2} + (k+1)^{2}&=\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6}\\
 \end{align}$$ 
It must be shown that 
$$
P(k)=\frac{k(k+1)(2k+1)}{6} \Rightarrow P(k+1)=\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6}
$$
Utilizing the induction hypothesis it is clear that $$ 1^{2}+2^{2}+3^{2} ...+((k+1)-1)^{2}=1^{2}+2^{2}+3^{2} ...+(k-1)^{2} + k^{2}$$
Substituting gives $$P(k+1)=\frac{k(k+1)(2k+1)}{6} + (k+1)^{2}\stackrel{?}{=}\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6}$$
With some algebra we need to show
$$\begin{align}
P(k+1)=\frac{k(k+1)(2k+1)}{6} + (k+1)^{2}&\stackrel{?}{=}\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6}\\


\end{align}$$
$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 
(To show that whatever statement is true for any positive integer $m$, show it is also true for the next integer $m+1$)

*Back work*
LHS
$$
\begin{align}
\frac{k(k+1)(2k+1)}{6}+(k+1)^{2}&=\frac{k(k+1)(2k+1)}{6}+\frac{k^{2}+2k+1}{1}\\
&=\frac{k(k+1)(2k+1)+6(k^{2}+2k+1)}{6}\\
&=\frac{k(2k^{2}+3k+1)+6(k^{2}+2k+1)}{6}\\
&=\frac{2k^{3}+3k^{2}+k+6k^{2}+12k+6)}{6}\\
&=\frac{2k^{3}+9k^{2}+13k+6}{6}\\
\end{align}$$
RHS
$$\begin{align}
\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6} &=\frac{(k+1)(k+2)(2k+3)}{6} \\
&=\frac{(k+1)(k+2)(2k+3)}{6} \\
&=\frac{(k^{2}+3k+2)(2k+3)}{6} \\
&=\frac{2k(k^{2}+3k+2)+3(k^{2}+3k+2)}{6} \\
&=\frac{2k^{3}+6k^{2}+4k+3k^{2}+9k+6}{6} \\
&=\frac{2k^{3}+9k^{2}+13k+6}{6} \\
\end{align}$$
Since it is shown that 
$$\frac{k(k+1)(2k+1)}{6}+(k+1)^{2}=\frac{(k+1)((k+1)+1)(2(k+1)+1)}{6} $$

$P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.
$\blacksquare$ 

---
#induction #algebra_proof 