### Notes
#### Methods of Proof by Induction:

[Induction Proofs, *Discrete Math* - Susan Epp](https://drive.google.com/file/d/1wTR6FQJE1Lv_3CG9ghrWdrpjR_CRfupc/view?usp=sharing)

If you are hoping to prove that an equation is true but you haven't yet done so, either preface it with words **"We Need To Show"** or put a question mark above the equal sign.

**Format 1 - the inductive step**: Start with the left hand side of the equation (LHS) to be proved and transform it using definitions, algebra, and (during the inductive step) the inductive hypothesis until you obtain the right-hand side of the equation (RHS).

**Format 2 - the basis step:** Transform the LHS and the RHS of the equation to be proved independently, one after the other, until both sides are shown to equal the same expression. 

**Format 3** - Similar to format 2 BUT computations are done in parallel. But in order to avoid the fallacy of assuming what is to be proved, do not put an equal sign between the two sides of the equation until the very last step. Separate the two sides of the equation with a vertical line

**Format 4** - Similar to 3, BUT sides are separated with a $\stackrel{?}{=}$ 

**Format 5 - iff:** Start by writing "We must show that" and give the equation you want to prove true. In successive steps, indicate that this equation is true, $\iff$ various other equations are true. BE SURE that both directions of the iff claim are correct. Because each subsequent equation is true iff the previous equation is true, then you will have shown the original equation is true. 

[Section 5.2 - 5.4, *Discrete Math* - Susan Epp]

#### Section 5.2 Notes
**Principle Of Mathematical Induction, PMI**: 

Let $P(n)$ be a property that is defined for integers $n$, and let a be a fixed integer. Suppose the following statements are true:

1st - $P(a)$ is true

2nd - For all integers $k \ge a$, if $P(k)$ is true then $P(k+1)$ is true.

Then the statement: *for all integers* $n \ge a,~~P(n)$ *is true.*

The validity of proof by mathematical induction is generally taken as an axiom. That is why it is referred to as the *principle of mathematical induction, PMI* rather than as a theorem. 

PMI is also equivalent to the following property about the set of integers. 

*Suppose S is any set of integers satisfying that* $a \in S$, *and for all integers* $k \ge a$, *if* $k \in S$ *then* $k+1$ *is in S*. *Then S must contain every integer greater than or equal to a.* 

Proving a statement by mathematical induction is a two step process: the **BASIS** step and the **INDUCTION** step

#### Insights:
1. **USE THE INDUCTIVE HYPOTHESIS**
2. **REARRANGE TO MAKE IT LOOK LIKE THE INDUCTION HYPOTHESIS**
3. **PROVEN FOR THE NEXT TERM IN SEQUENCE, PROVEN FOR ENTIRE SEQUENCE**

**Toolbox**

To construct a proof by induction, you must first identify the property $P(n)$.

In the **BASIS** step of the proof, you must show that the property is true for $n =a$, or in other words that $P(a)$ is true. *plug in some # for* $P(n)$, *verify that LHS = RHS* $\checkmark$ 

In the **INDUCTIVE** step of the proof, you assume that $P(k)$ is true for an arbitrary integer $k$ that is close to $a$, given by $k \ge a$. This is called the #inductive_hypothesis. $P(k+1)$ is gained then by substituting $k+1$ into $P(k)$

*During the inductive step, a substitution or a* #magic_factor *is often used to get* $P(k+1)$ *in terms of* $P(k)$. 

**Classic Induction Proofs**
1. Formulas
2. Patterns (Series and Sequences)
3. Closed form of a series - the general forms for 2
4. Property - divisibility, prime numbers, etc.

#equality statements will often involve an #algebra_proof or utilizing a #magic_factor 

- Combining and splitting like terms
- Factoring
- Fractions
- Radicals
- Exponential Rules
- Trig Identities

With #inequalities statements, they will often involve creating a logical ordered statement like: "this is less than that, so this other thing must be is less than that too"

**Induction Process**

"Does $P(k)$ hold $\forall k \in S$? If it does, we can use $P(k)$ to show that $P(k+1)$ holds and thus P(n) is true."

### Proof Outline:
Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true

**BASIS STEP:** Let $n=1$ *(To show that* $P(n)$ *is true)* 

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$

*We Need To Show:* $P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

### Example 1:
Show that $2^{3n+1} +5$ is always a multiple of 7. #manipulate_powers

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

**BASIS STEP:** Let $n=1$ (To show that $P(n)$ is true) 

$$2^{3(1)+1}+5=2^{4}+5=21$$
21 is a multiple of 7. 

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:**

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k\ge 1$

*We Need To Show:* $P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align}
P(k)&=2^{3k+1} +5 \\
P(k+1)&=2^{3(k+1)+1}+5\\
P(k+1)&=2^{3k+4}+5
\end{align}$$

It follows that in order for $P(k+1)$ to be true, it must be a multiple of 7, given by $7x$

*We Need to Show:* $2^{3k+4} +5 \stackrel{?}{=} 7x$

$$\begin{align}
2^{3k+4} +5&=2^{3k} \cdot 2^4 +5~~~\text{by the rules of exponents}\\
&=2^{3k}(16)+5\\
&=2^{3k}(14+2)+5\\
&=2^{3k}(14)+2^{3k}(2)+5~~~\text{by the distributive property}\\
&=2^{3k}(14)+2^{3k+1}+5\\
\end{align}$$

#magic_factor It is given that $2^{3k}(14)$ is divisible by 7 and it is also assumed that $2^{3k+1}+5$ is divisible by 7. In addition, it is known that the sum of a number's multiples yields a multiple of that number, therefore it follows that $P(k+1)=2^{3k+4}+5=2^{3(k+1)}+5$ is divisible by 7.  

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

$\blacksquare$

[[Methods of Proof A.8.3 Proof by Induction]]

### Example 2: 
Show that $$1+2+3+...+(n-1)+n=\frac{n(n+1)}{2}$$ #algebra_proof 

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

**BASIS STEP:** Let $n=1$ (To show that $P(n)$ is true) 

$P(1)=\frac{1(1+1)}{2}=\frac{2}{2}=1$

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.


**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k\ge 1$

$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align}
P(k)&=1+2+3+...+(k-1)+k=\frac{k(k+1)}{2}\\
P(k+1)&=1+2+3+...+((k+1)-1)+(k+1)=\frac{(k+1)((k+1)+1)}{2} \\
&=1+2+3+...+(k-1)+k+(k+1)=\frac{(k+1)((k+1)+1)}{2} \\
\end{align}$$

Since $1+2+3+...+(k-1)+k=\frac{k(k+1)}{2}$, with some algebra

$$\begin{align}
P(k+1)&=\frac{k(k+1)}{2}+(k+1)\stackrel{?}{=}\frac{(k+1)((k+1)+1)}{2} \\
&=\frac{k(k+1)}{2}+\frac{2(k+1)}{2}=\frac{(k+1)((k+1)+1)}{2} \\
&=\frac{k(k+1)+2(k+1)}{2}=\frac{(k+1)((k+1)+1)}{2} \\
&=\frac{(k+1)(k+2)}{2}=\frac{(k+1)((k+1)+1)}{2} \\
&=\frac{(k+1)((k+1)+1)}{2}=\frac{(k+1)((k+1)+1)}{2} ~~\checkmark\\
\end{align}$$

Since both sides of the equation are equal it follows that $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

[[Methods of Proof A.8.1 Proof by Induction]]

### Example 3:
Show that $$1+3+5+...+(2n-1)=n^2$$ #algebra_proof 

Proof: 

Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

**BASIS STEP:** Let $n=1$ (To show that $P(n)$ is true)

$P(1)=(2(1)-1)=(2-1)=1=1^2=1$

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k\ge 1$

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align}
P(k)&=1+3+5+...+(2k-1)=k^2\\
P(k+1)&=1+3+5+...+(2(k+1)-1)\stackrel{?}{=}(k+1)^2\\
\end{align}$$

It follows that for $P(k+1)$ to be true it must be equal to $(k+1)^2$

With some algebra:

$$\begin{align}
P(k+1)&=1+3+5+...+(2(k+1)-1)\stackrel{?}{=}(k+1)^2\\
&=1+3+5+...+(2k+1)\stackrel{?}{=}(k+1)^2\\
&=1+3+5+...+(2k-1)+(2k+1)\stackrel{?}{=}(k+1)^2
\end{align}$$

*We Need To Show:*  $P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

Since $P(k)=1+3+5+...+(2k-1)=k^2$, substituting gives

$$\begin{align}
P(k+1)&=1+3+5+...+(2k-1)\stackrel{?}{=}(k+1)^2\\
P(k+1)&=k^2+(2k+1)\stackrel{?}{=}(k+1)^2\\
P(k+1)&=k^2+2k+1=(k+1)^2\end{align}$$

Since both sides of the equation are equal, it follows that $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

### Example 4:
Prove $3^n \ge 2n+1~~~ \forall n \in \mathbb{Z}^+$ #inequalities 

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

**BASIS STEP:** Let $n=1$ (To show that $P(n)$ is true) 

$P(n)=3^{n}\ge 2n+1$

$P(1)=3^{1} \ge 2(1)+1$

$=3\ge 3~\checkmark$

$\therefore~P(1)$ is true and $1\in S$ so $S$ is not empty.

**INDUCTION STEP:**

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 1$

$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align}
P(k)&=3^{k}\ge 2k+1\\
P(k)&=3^{k+1}\ge 2(k+1)+1\\
\end{align}$$

It follows that $3^{k+1}=3^{k} \cdot 3$ and given that $3^{k}>2k+1$ it can be said that: 

$$\begin{align}
3^{k+1}&=3^{k}\cdot 3\\
&\ge (2k+1) \cdot 3=3\cdot 2k +3 \hspace{1cm} \textit{distributive property}\\
&\ge 3 \cdot 2k + 3
\end{align}$$

Given that $3^{k}\ge 2k+1$ and it is shown that $3^{k+1} \ge 3 \cdot 2k+3$ surely it can be said that because $3 \cdot 2k +3 \ge 2k +3$,

$$\begin{align}
3^{k+1} &\ge 2k+3\\
3^{k+1} &\ge 2k+2+1\\
3^{k+1} &\ge 2(k+1)+1\\
\end{align}$$ 
Then it is shown that $$3^{k+1}\ge 2(k+1)+1$$

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

### Example 5: 

Show that for all integers, $n\ge 3$, $2n+1 < 2^n$  #inequalities 

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

**BASIS STEP:** Let $n=3$ (To show that $P(n)$ is true) 

$P(n)=2n+1<2^n$

$P(3)=2(3)+1<2^{3}$

$=7<8~\checkmark$

$\therefore P(3)$ is true and $3\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 3$

$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

*(To show that whatever statement is true for any positive integer* $m$, *show it is also true for the next integer* $m+1$)

$$\begin{align}
P(k)&=2k+1<2^k\\
P(k+1 )&=2(k+1)+1<2^{k+1}\\
\end{align}$$

It follows that $2^{k+1}=2^{k} \cdot 2$ and given that $2^{k}>2k+1$ it can be said that: 

$$2^{k}\cdot 2 > (2k+1)\cdot 2$$

With some algebra

$$\begin{align}
2^{k}\cdot 2 &> (2k+1)\cdot 2 \\
&=4k+2 \\
&= 2\cdot 2k +2 \\
\end{align}$$

Since $2(k+1)+1=2k+3$, surely it can be said that 

$$\begin{align}
2\cdot 2k+2&>2k+3, \forall k\ge 3 \\
2\cdot 2k+2&>2k+2+1\\
2\cdot 2k+2&>2(k+1)+1\\
\end{align}$$
 
and given that 

$$P(k)=2k+1<2^{k}$$

It follows that

$$2^{k+1}>2(k+1)+1$$

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.


### Example 6 : 
Prove that $P(n): n^{2}\ge 2n+3, n\ge 3$ #inequalities 

Proof: Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true 

**BASIS STEP:** Let $n\ge 3$ (To show that $P(n)$ is true) 

$$\begin{align}
3^{2}&\ge 2(3)+3 \\
9&\ge 9~~~\checkmark\\
\end{align}$$

$\therefore~P(3)$ is true and $3\in S$ so $S$ is not empty.

**INDUCTION STEP:** 

Induction Hypothesis: Assume $P(k)$ is true and that the statement holds for $n=k$, and $k \ge 3$

$P(k) \Rightarrow P(k+1)$ , $\forall k \in S$ 

(To show that whatever statement is true for any positive integer $m$, show it is also true for the next integer $m+1$)

$$\begin{align}
P(k)&=k^{2} \ge 2k+3\\
P(k+1)&=(k+1)^{2} \ge 2(k+1)+3\\
\end{align}$$

Given that  $k^{2} \ge 2k+3$ and $(k+1)^2 = k^2+2k+1$,  it can be said that  $(k+1)^{2}=k^2+2k+1 \ge (2k+3)+2k+1$

Then with some algebra

$$\begin{align}
(k+1)^{2} &\ge (2k+3)+2k+1\\
(k+1)^{2} &\ge (2k+3)+2k+1\\
(k+1)^{2} &\ge 4k+4 \\
(k+1)^{2} &\ge 2\cdot 2k+4 \\
\end{align}$$

Given that $2(k+1)+3=2k+5$ and $(k+1)^{2} \ge 4k+4$, surely it can be said that

$$\begin{align}
2\cdot 2k+4 &> 2k +5,~~~\forall k\ge 3\\
(k+1)^{2}&> 2k+5 \\
(k+1)^{2}&> 2k+2+3 \\
(k+1)^{2}&> 2(k+1)+3 \\
\end{align}$$

It is shown that 

$P(k+1)=(k+1)^{2} \ge 2(k+1)+3$

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

---

#induction #proof 