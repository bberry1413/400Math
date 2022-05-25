[[Methods of Proof Induction Proof Insights]]

Prove by induction that for every $n=1,2,3,...$ $$(1+x)^n \ge 1 + nx$$ for any $x>0$.

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true

**BASIS STEP:** Let $n=1$ *(To show that* $P(n)$ *is true)* 

$P(n)=(1+x)^n \ge 1+nx$

$P(1)=(1+x)^1 \ge 1+1x$

$1+x \ge 1+1x ~\checkmark$

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$

*We Need To Show:* $P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align}
P(k)&=(1+x)^k \ge 1+kx\\
P(k+1)&=(1+x)^{k+1} \ge 1+(k+1)x\\
\end{align}$$

We Need To Show 
$$(1+x)^{k+1} \stackrel{?}{\ge} 1+ x +kx$$


It follows that $(1+x)^{k+1}=(1+x)^{k}(1+x)$ and given that $(1+x)^k \ge 1+kx$ it can be said that

$$\begin{align}
(1+x)^{k+1}&=(1+x)^{k}(1+x) \\
&\ge (1+kx)(1+x)=1+x+kx+kx^2\\
\end{align}$$

Rearranging gives

$$\begin{align}
(1+x)^{k+1}&\ge 1+x+kx+kx^2\\
&\ge (1+kx)+(x+kx^2)
\end{align}$$

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.
