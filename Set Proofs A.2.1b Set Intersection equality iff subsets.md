### Show that $A \cap B = A \iff A \subset B$ 
_To show $A\cap B = A$, show $A\cap B\subset A$ and $A\subset A\cap B$_

**Set Equality Proof Frame**
1. Let $x\in A\cap B$
2. Show $A \cap B \subset A$
	**Subset Proof Frame**
	1. Let $x \in A\cap B$
	2. Show $x\in A$
	3. Then $A\cap B\subset A \hspace{1cm}\blacksquare$
3. Let $y\in A$
4. Show $A\subset A \cap B$
	**Subset Proof Frame**
	1. Let $y \in A$
	2. Show $y\in A \cap B$
	3. Then $A\subset A \cap B\hspace{1cm}\blacksquare$
5. If $A\cap B \subset A$ and $A \subset A \cap B$, then $A \cap B = A \hspace{1cm}\blacksquare$
<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>
#### Proof:
$\Leftarrow$ Given $A\subset B$
_Show $A\cap B = A$_

Let $x\in A\cap B$ and given that $A\subset B$
Implications
1. If $x\in A\cap B$ , $x \in A$ and $x\in B$ by definition of intersection of sets.

Since $x \in A \cap B$ and $x \in A$, it follows that $A\cap B \subset A$

Let $y\in A$ and given that $A\subset B$
Implications
1. If $y\in A$, and $A\subset B$, it follows that $y\in B$
2. If $y\in A$ and $y \in B$, by definition of intersection, $y \in A\cap B$ 
Since $y\in A$ and $A \subset B$ and it is shown that $y\in A\cap B$ and $A \subset A \cap B$ 

Therefore, given that $A \subset B$, and it is shown that $A \cap B \subset A$  and $A\subset A\cap B$ , then $A \cap B = A$. 

$\Rightarrow$ Given $A\cap B = A$
_Show $A\subset B$_

Let $x\in A$
Implications
1.  Given that $A\cap B =A$, if $x \in A$, then $x\in B$ by definition of intersection.
2. Since $x\in A$, and it is shown that $x\in B$, then $A \subset B$

Therefore, $A\cap B = A \Leftarrow \Rightarrow A \subset B$
$\blacksquare$

---
#sets #subsets #intersection #set_equality #proof 