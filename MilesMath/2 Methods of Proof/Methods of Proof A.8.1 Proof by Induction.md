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
Compute for $n=1,2,3,4$, and $5$ the value of $$1+3+5+...+(2n-1).$$
This should be enough values to suggest a correct formula. Verify it by induction.

---
Prove by induction for every $n=1,2,3,...$ that the number $$7^n-4^n$$ is divisible by 3. 


---
Prove by induction that for every $n=1,2,3,...$ $$(1+x)^n \ge 1 + nx$$ for any $x>0$.

---
Prove by induction that for every $n=1,2,3,...$ that $$1+r+r^2+...+r^n = \frac{1-r^{n+1}}{1-r}$$ for any real number $r \ne 1$.

---
Prove by induction that for every $n=1,2,3,...$ that $$1^3 + 2^3 + 3^3 + ...+n^3 = (1+2+3+...+n)^2$$

---
Prove by induction that for every $n=1,2,3,...$ that $$\frac{d^{n}}{dx^{n}}e^{2x}=e^{2x+n\log 2}.$$

---
Show that the following two principles are equivalent (i.e., assuming the validity of one of them, prove the other). 
	**(Principle of Induction)** Let $S \subset \mathbb{N}$ such that $1 \in S$ and for all integers $n$ if $n \in S$, then so is $n+1$. Then $S = \mathbb{N}$.
	**(Well Ordering of $\mathbb{N}$)** If $S \subset \mathbb{N}$ and $S \ne \emptyset$ , then $S$ has a first element (i.e., a minimal element) well ordering of $\mathbb{N}$