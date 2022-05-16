### Show that $\mathbf{A\cup B = B \iff A \subset B}$ 
_To show sets $A\cup B = B$, show $A\cup B\subset B$ and $B\subset A \cup B$_
_Try to prove $\iff$ statements both ways_

**Set Equality Proof Frame**
1. Let $x\in A\cup B$
2. Show $A \cup B \subset B$
	**Subset Proof Frame**
	1. Let $x \in A\cup B$
	2. Show $x\in B$
	3. Then $A\cup B\subset B \hspace{1cm}\blacksquare$
3. Let $y\in B$
4. Show $B\subset A \cup B$
	**Subset Proof Frame**
	1. Let $y \in B$
	2. Show $y\in A \cup B$
	3. Then $B\subset A \cup B\hspace{1cm}\blacksquare$
5. If $A\cup B \subset B$ and $B \subset A \cup B$, then $A \cup B = B \hspace{1cm}\blacksquare$

<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>

#### Proof: 
$\Leftarrow$ Given $A\subset B$ 
_To show $A\cup B = B$, show $A\cup B\subset B$ and $B\subset A\cup B$_ 

Let $x\in A \cup B$ and given that $A \subset B$,
Implications
1. If $x \in A \cup B$, then $x\in A$, $x \in B$, or $x \in A \cap B$ 
2. If $x\in B$, or $x \in A \cap B$, it follows that $x\in B$ 
3. If $x\in A$, and $A \subset B$ it follows $x \in B$ and $A \cup B \subset B$ 

Since $x \in A \cup B$ and $A\subset B$, it can be concluded that $x\in B$ and $A\cup B \subset B$ by definition of subsets.

Let $y \in B$ 
Implications
1. $y\in B$ if follows that $y \in A \cup B$ by definition of union of sets. 

Since $y\in B$ and $A\subset B$, it can be concluded that  $y \in A \cup B$, and $B \subset A \cup B$  by definition of subsets.

Therefore, given that $A \subset B$, and it is shown that $A \cup B \subset B$  and $B\subset A\cup B$ , then $A \cup B = B$. 

$\Rightarrow$ Given $A \cup B = B$ 
_Show $A\subset B$_
Let $x \in A$
Implications
1. If $x \in A \cup B$, by the definition of the union of sets $x \in A$ or $x\in B$
2. However by assumption, $A \cup B = B$, then it follows that $x \in B$.
Since $x \in A$ and it is shown that $x\in B$, $A \subset B$ 

Therefore, $A \cup B = B \iff A \subset B$ 
$\blacksquare$

---
#sets #subsets #union #set_equality #proof 