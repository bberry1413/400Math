## Methods of Proof: A.5.1, A.6.1, A.7.1, A.7.2, A.7.3, A.8.1, A.8.2, A.8.5, A.9.1, A.9.3, A.9.4
#### MA 403 - Advanced Calculus - Brandiece Berry

### A.5.1) Show that $\sqrt{2}$ is irrational by giving an indirect proof

#### Proof:
Assume $\sqrt{2}$ is rational. Then by definition, $\sqrt{2}=\dfrac{a}{b}$ where  $a\in \mathbb{Z}$ and $b \in \mathbb{N}$. Let us also assume that $\dfrac{a}{b}$ is in simplest terms, that is that a and b have no common factors. The expression can be rewritten as: $2=\dfrac{a^2}{b^2}$ and finally as, $2b^2=a^2$ .  It follows that by definition, a is an even number and b is a multiple of a, meaning it is also an even number. But it was given that a is not a multiple of b, and here lies the contradiction $\rightarrow \leftarrow$
$\therefore$ by proof by contradiction, $\sqrt{2}$ is irrational.

_This proof relies on the definition of a rational number: r is rational if r = a/b for some integers a and b, with b ne 0. We may assume that a and b have no common factors because otherwise, we would simply reduce a/b by canceling all common factors._

#proof #indirect_proof #irrational 

---
### A.6.1) Prove the following assertion by contraposition: If x is irrational, then $x+r$ is irrational for all rational numbers $r$.
If-Then statement: If **x is irrational** then **x+r is irrational for all rational numbers.**
The Contrapositive: If **$x+r$ is rational for all rational numbers $r$**, then **$x$ is rational.**

Then there exists $\frac{a}{b}$ such that $x+r=\frac{a}{b}$. It is given that $r$ is already a rational number, let it be given by $\frac{p}{q}$, and therefore $x$ can be written as:
$x=\frac{a}{b} - \frac{p}{q}$
$x=\frac{aq-bp}{bq}=\frac{w}{z}$ where $a,b,p,q,w,z \in \mathbb{Z}$
$\therefore$ by proof by contrapositive, if $x$ is irrational, $x+r$ is irrational for all rational numbers $r$. 
$\blacksquare$

#irrational #proof #contrapositive #if_then #algebra_proof 

---
### A.7.1) Disprove the statement: For any natural number $n$ the equation $$4x^{2}+x -n=0$$ has no rational root.

To disprove this statement, a counterexample is given. 

Let's assume there is a rational root that satisfies this equation. Meaning, some number for $n$ will provide a rational root for the equation. Consider one possible root:

$x= \frac{-1+\sqrt{(1)^2-4(4)(-n)}}{2(4)}=\frac{a}{b}$

With some algebra
$$\begin{align}
\frac{-1+\sqrt{1+16n}}{8}&=\frac{a}{b}\\

-1 + \sqrt{1+16n}&=\frac{8a}{b}\\
\sqrt{1+16n}&=\frac{8a}{b}+1\\
\sqrt{1+16n}&=\frac{8a+b}{b}\\
1+16n&=\left(\frac{8a+b}{b}\right)^2\\
16n&=\left(\frac{8a+b}{b}\right)^{2}-1\\
16n&=\frac{64a^{2}+16ab +b^2}{b^{2}}-1\\
16n&=\frac{64a^{2}+16ab +b^2}{b^{2}}-\frac{b^2}{b^2}\\
16n&=\frac{64a^{2}+16ab}{b^{2}}\\
n&=\frac{64a^{2}+16ab}{16b^{2}}\\
n&=\frac{4a^2+ab}{b^{2}}\\
\end{align}$$
Let a = 1 and b = 2
$$n=\frac{4(1)^2+(1)(2)}{2^2}=\frac{3}{2}$$
And so the polynomial $4x^{2}+x- \frac{3}{2}=0$ will have rational roots: $x_{1}= \frac{1}{2}, x_{2} =- \frac{3}{4}$.

#irrational #rational_root #algebra_proof #counterexample 

---
### A.7.2) Every prime greater than two is odd. Is the converse true?

If-Then Statement: If **a prime number is greater than two** then **it is odd**.

The Converse: If **a number is odd**, then **it is a prime number greater than two**.

Proof by Counterexample:
This is false. 15 is an odd number greater than 2 that is not prime.
 
#proof #counterexample #prime #odd #converse 

---
### A.7.3) State both the converse and the contrapositive of the assertion "Every differentiable function is continuous." Is there a difference between them? Are they both true?

If-Then Statement: If **a function is differentiable**, then **it is continuous.**

Converse: If **a function is continuous**, then **it is differentiable.**

This is not always true and can be disproved with a counterexample:
$f(x)=|x|$ is an example of a continuous function that is not differentiable.


Contrapositive: If **a function is not continuous**, then **it is not differentiable.** 

Since the original conditional statement is true then the contrapositive is also true. A function that is not continuous is also not differentiable. 

#proof #contrapositive #converse #differentiable #continuous

--- 
A.8.1)
A.8.2)
A.8.5)

---
### A.9.1) ### Let $\mathbb{R}$ be as usual the set of all real numbers. Express in words what these statements mean and determine whether they are true or not. Do not give proofs; just decide on the meaning and whether you think they are valid or not.

- (a) $\forall x\in \mathbb{R}, x\ge 0$
This statement is false because it means, "Every x that is in the set of all real numbers must be greater than or equal to zero." The set of real numbers includes numbers less than zero.

- (b) $\exists x\in \mathbb{R}, x\ge 0$
This statement is true because it means, "There exists a number $x \ge 0$ that resides in $\mathbb{R}$."

- (c) $\forall x\in \mathbb{R}, x^{2}\ge 0$
This statement is true because it means "Every $x$ within $\mathbb{R}$ has a square that is greater than or equal to zero." Even the smallest numbers or the most negative numbers within $\mathbb{R}$ will have a square greater than or equal to zero.   

- (d) $\forall x\in \mathbb{R},\forall y\in \mathbb{R}, x+y=1$
This statement is false because it means, "Every $x$ and $y$ in $\mathbb{R}$ has a sum equal 1. " There will be other sums other than 1 for all $x$ and $y$ in $\mathbb{R}$.

- (e) $\forall x\in \mathbb{R},\exists y\in \mathbb{R}, x+y=1$
This statement is true because it means, "Every $x$ and some $y$ in $\mathbb{R}$ have a sum equal 1." Any number within $\mathbb{R}$ has another number that can be added to it and the sum will be 1.

- (f) $\exists x\in \mathbb{R},\forall y\in \mathbb{R}, x+y=1$
This statement is false because it means, "Some number $x$ and every $y$ in $\mathbb{R}$ have a sum equal 1."  There will be an $y$ in $\mathbb{R}$ where a $x$ cannot be added to it to equal 1.

- (g) $\exists x\in \mathbb{R},\exists y\in \mathbb{R}, x+y=1$
This statement is true because it means "Some $x$ and some $y$ in $\mathbb{R}$ have a sum equal 1." There are several examples: $x=0.2$ and $y =0.8$ is one example.

---
#quantifiers #for_all #there_exists #Reals

---
### A.9.3) Explain what must be done in order to prove an assertion of the following form: (a) $\forall s\in S$ "statement about s" is true. (b) $\exists s\in S$ "statement about s" is true.

- (a) $\forall s\in S$ "statement about s" is true.
In order to prove a "for all" statement is true, every element of S must hold true for the "statement about s."

- (b) $\exists s\in S$ "statement about s" is true.
In order to prove a "there exists" statement is true, only 1 element of S must hold true for the "statement about s."

In order to disprove a "for all" statement, a "there exists" statement will be used to show that at least one element of S does not fit the "statement about s."

In order to disprove a "there exists" statement, a "for all" statement will be used to show that not one element of S fits the "statement about s." 

#proof #for_all #there_exists #sets

---
### A.9.4) In the preceding exercise suppose that $S=\emptyset$. Could either statement be true? Must either statement be true?

The "for all" statement could be true. The statement could be $\forall s\in S, S=\emptyset$.
The "there exists" statement is always false because there is nothing to verify that "there exists" within the empty set. 

No, both statements do not need to be true. 

#sets #empty_set #for_all #there_exists 