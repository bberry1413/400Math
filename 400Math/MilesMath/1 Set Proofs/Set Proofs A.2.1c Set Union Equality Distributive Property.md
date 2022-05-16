### Show that $(A\cup B)\cap C = (A\cap C)\cup (B\cap C)$
_To show two sets are equal, show they are subsets of each other_
Show $(A \cup B)\cap C \subset (A\cap C)\cup (B\cap C)$ and $(A\cap C)\cup (B\cap C) \subset (A \cup B)\cap C$

**Set Equality Proof Frame**
1. Let $x \in (A \cup B)\cap C$
2. Show $(A\cup B)\cap C \subset (A\cap C)\cup (B\cap C)$
	**Subset Proof Frame**
	1. Let $x \in (A \cup B)\cap C$
	2. Show $x\in (A\cap C)\cup (B\cap C)$
	3. Then $(A\cup B)\cap C \subset (A\cap C)\cup (B\cap C)$
	$\blacksquare$
3. Let $y\in (A\cap C)\cup (B\cap C)$
4. Show $(A\cap C)\cup (B\cap C) \subset (A\cup B)\cap C$
	**Subset Proof Frame**
	1. Let $y \in (A\cap C)\cup (B\cap C)$
	2. Show $y\in (A\cup B)\cap C$
	3. Then $(A\cap C)\cup (B\cap C) \subset (A\cup B)\cap C$
	$\blacksquare$
5. If $(A\cup B)\cap C \subset (A\cap C)\cup (B\cap C)$ and $(A\cap C)\cup (B\cap C) \subset (A\cup B)\cap C$, then $(A\cup B)\cap C = (A\cap C)\cup (B\cap C)$
$\blacksquare$

#### Proof:
Let $x\in (A \cup B)\cap C$
Implications
1. If $x\in (A\cup B)\cap C$, then the following must be true:
	1. $x\in (A\cup B)\cap C$, $x\in A\cup B$ and $x\in C$ by definition of the intersection of sets.
	2. $x \in A\cup B$, and therefore $x\in A$ or $x\in B$ by definition of the union of sets.
2. Since $x\in (A\cup B)\cap C$, $x\in A$ or $x\in B$ and $x\in C$, it follows that if
	1. $x\in A$ and $x\in C$, then $x\in A\cap C$
	2. $x\in B$ and $x\in C$, then $x\in B\cap C$
3. It is shown that if $x\in A\cup B$ and $x\in C$, $x\in A\cap C$ or $x\in B\cap C$
	1. By definition of the union of sets it follows that $x\in (A\cap C) \cup (B \cap C)$

It follows that $(A \cup B)\cap C \subset (A\cap C)\cup (B\cap C)$

Let $y\in (A\cap C)\cup (B\cap C)$
Implications
1. If $y\in (A\cap C)\cup (B\cap C)$, $y\in A\cap C$ or $y\in B\cap C$, by definition of the union of sets.
2. Since $y\in A\cap C$ or $y\in B\cap C$
	1. $y\in A$ and $y\in C$ 
	2. $y\in B$ and $y\in C$
3. Since it is shown that $y\in C$, and $y\in A$ or $y\in B$, by definition $y\in (A\cup B)\cap C$

It follows that $(A\cap C)\cup (B\cap C)\subset (A \cup B)\cap C$
Therefore,
$(A\cup B)\cap C = (A\cap C)\cup (B\cap C)$
$\blacksquare$
---
#sets #subsets #set_equality #intersection #union #proof 