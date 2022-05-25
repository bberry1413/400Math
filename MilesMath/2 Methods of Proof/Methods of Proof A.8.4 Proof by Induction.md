[[Methods of Proof Induction Proof Insights]]

Prove by induction that for every $n=1,2,3,...$ $$(1+x)^n \ge 1 + nx$$ for any $x>0$.

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true

**BASIS STEP:** Let $n=1$ *(To show that* $P(n)$ *is true)* 

$P(n)=(1+x)^n \ge 1+nx$

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$

*We Need To Show:* $P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.
