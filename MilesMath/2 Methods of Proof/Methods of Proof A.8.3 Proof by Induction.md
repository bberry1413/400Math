Prove by induction for every $n=1,2,3,...$ that the number $$7^n-4^n$$ is divisible by 3. 

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 
BASIS STEP:
Let $n=1$ *(To show that $P(n)$ is true)* 
$P(n)=7^n-4^{n} = 3x$

$P(1)=7^{1}-4^{1}=7-4=3$ and $\frac{3}{3}= 1~~\checkmark$

$\therefore P(1)$ is true and $1\in S$ so $S$ is not empty.

INDUCTION STEP: 
Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$
$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 
*(To show that whatever statement is true for any positive integer $m$, show it is also true for the next integer $m+1$)*
$$\begin{align}
P(k)&=7^{k}-4^{k}=3x\\
P(k+1)&=7^{k+1}-4^{k+1}=3x \\
\end{align}$$

Rewriting $P(k)$ with $\ln x$ 

$$\begin{align}
P(k)&=7^{k}-4^{k}=3x\\
k\ln7 -k\ln4&=\ln(3x) \\
k(\ln7 -\ln4)=\ln3+\ln x \\
\end{align}$$

$$\begin{align}
7^{k+1}-4^{k+1}&= (k+1)\ln 7 - (k+1) \ln 4 \\
&=k\ln7 +\ln7 -k\ln4-\ln4 \\
&=k\ln7 - k\ln4+\ln7-\ln4 \\
&=k(\ln7-\ln4) +\frac{\ln7}{\ln4}
\end{align}$$


So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 
 
$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.