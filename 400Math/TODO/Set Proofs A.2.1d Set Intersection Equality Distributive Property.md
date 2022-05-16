### Show that $(A\cap B)\cup C=(A\cup C)\cap (B\cup C)$
_To show two sets are equal, show they are subsets of each other_
Show $(A\cap B)\cup C \subset (A\cup C)\cap (B\cup C)$ and $(A\cup C)\cap (B\cup C)\subset (A\cap B)\cup C$

**Set Equality Proof Frame**
1. Let $x \in (A \cap B)\cup C$
2. Show $(A\cap B)\cup C \subset (A\cup C)\cap (B\cup C)$
	**Subset Proof Frame**
	1. Let $x \in (A \cap B)\cup C$
	2. Show $x\in (A\cap C)\cup (B\cap C)$
	3. Then $(A\cap B)\cup C \subset (A\cup C)\cap (B\cup C)$
	$\blacksquare$
3. Let $y\in (A\cup C)\cap (B\cup C)$
4. Show $(A\cup C)\cap (B\cup C)\subset (A\cap B)\cup C$
	**Subset Proof Frame**
	1. Let $y\in (A\cup C)\cap (B\cup C)$
	2. Show $y\in (A \cap B)\cup C$
	3. Then $(A\cup C)\cap (B\cup C)\subset (A\cap B)\cup C$
	$\blacksquare$
5. If $(A\cap B)\cup C \subset (A\cup C)\cap (B\cup C)$ and $(A\cup C)\cap (B\cup C)\subset (A\cap B)\cup C$, then $(A\cap B)\cup C=(A\cup C)\cap (B\cup C)$
$\blacksquare$

#### Proof:
Let $x \in (A \cap B)\cup C$
Implications
1. If $x \in (A \cap B)\cup C$, then the following must be true:
	1. $x \in (A \cap B)\cup C$, $x\in A\cap B$ or $x\in C$, by definition of the union of sets
	2. $x\in A\cap B$, and therefore $x \in A$ and $x\in B$, by definition of intersection of sets
2. Since $x \in (A \cap B)\cup C$, $x\in A\cap B$ or $x\in C$, it follows that if
		1. $x\in A$ or $x\in C$, then $x \in A\cup C$
		2. $x\in B$ or $x\in C$, then $x \in B\cup C$
3. Because $x\in A\cap B$, if $x\in A\cup C$ and $x\in B\cup C$, it follows that $x \in (A\cup C) \cap (B \cup C)$ by definition of the intersection of sets.

It follows that $(A\cap B)\cup C \subset (A\cup C)\cap (B\cup C)$

Let $y\in (A\cup C)\cap (B\cup C)$ 
Implications
1. If $y\in (A\cup C)\cap (B\cup C)$, $y \in A \cup C$ and $y \in B\cup C$ by definition of the intersection of sets
2. If $y \in A \cup C$, it follows that $y\in A$, $y\in C$ or $y\in A\cap C$ by definition of union of sets
3. Since $y\in A\cup C$,  $y\in A$, $y\in C$ or $y\in A\cap C$, it follows that if
	1. 