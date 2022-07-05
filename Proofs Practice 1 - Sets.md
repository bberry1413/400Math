#### Subsets: Proof and Disproof
#EppsDiscreteMath 

Begin by writing what it means for a set A to be a subset of set B as a formal universal conditional statement: $$ A \subset B \iff \forall x \in A~~ \text{then}~ x \in B$$ 
1. Suppose that $x \in A$
2. Show that x is also $x \in B$

EX] Sets A and B are defined as follows: $$\begin{align} A &=\{m \in \mathbb{Z}~|~m=6r+12~~\text{for some}~r \in \mathbb{Z}\}\\
B &=\{n \in \mathbb{Z}~|~n=3s~~\text{for some}~s \in \mathbb{Z}\} \end{align}$$
Prove  $A \subset B$
1. Let $x \in A$ and a random element of A. 
	_1. We must show that $x \in B$. By definition this means x = c_
2. By definition of set A, there is an integer r such that $x=6r+12$ 
	_1. We need a way to link set A to set B through definitions._
	_2. We can rewrite set A as $x=3(2r+4)$_
3. By definition of set B, we know that n is given by $n=3s$. 
4. Let $s=2r +4$ in order to link set A and set B (get one in terms of the other)
	_1. Since it was given that r is an integer, by definition of integer multiplication and addition, 2r+4 will also be an integer, so we can conclude that s is an integer_
5. If  $s=2r +4$, then $3s$ = $6s+12$ = x. 
6. Since B is defined by $n=3s$ and $x \in A$, and can be written as the product of $3s$, it follows that $x \in B$ and $A \subset B$  $\blacksquare$

Disprove $B \subset A$
1. Let $x \in A$ and a random element of A. 
	_1. We must show that $x \in B$. By definition this means x = c_
