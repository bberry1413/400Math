Prove by induction for every $n=1,2,3,...$ that the number $$7^n-4^n$$ is divisible by 3. 

#manipulate_powers 

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

BASIS STEP: Let $n=1$ (To show that $P(n)$ is true) 

$P(n)=7^n-4^{n} = 3x$

$P(1)=7^{1}-4^{1}=7-4=3$ and $\frac{3}{3}= 1~~\checkmark$

$\therefore P(1)$ is true and $1\in S$ so $S$ is not empty.

INDUCTION STEP: 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$

$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

(To show that whatever statement is true for any positive integer $m$, show it is also true for the next integer $m+1$)

$$\begin{align}
P(k)&=7^{k}-4^{k}\\
P(k+1)&=7^{k+1}-4^{k+1} \\
\end{align}$$
It follows that in order for $P(k+1)$ to be true, it must be a multiple of 3, given by $3x$

*We Need To Show:* $7^{k+1}-4^{k+1} \stackrel{?}{=} 3x$

Rewriting $P(k+1)$

$$\begin{align}
7^{k+1}-4^{k+1}&=7^{k}\cdot 7 -4^{k}\cdot 4\\
&=(7^k)(3+4)-4^k(4)\\
&=7^k(3)+7^k(4)-4^k(4)\\
&=7^k(3)+4(7^k-4^k)\\
\end{align}$$

#magic_factor It is given that $7^k(3)$ is divisible by 3 and since it is also assumed that $7^k-4^k$ is divisible by 3, $4(7^k-4^k)$ is also divisible by 3 because it is a multiple of 3.

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 
 
$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

$\blacksquare$