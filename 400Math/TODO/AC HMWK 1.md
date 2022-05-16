### Sets: A.2.1, A.2.2, A.2.3
#### MA 403 - Advanced Calculus - Brandiece Berry

### A.2.1a) Show that $\mathbf{A\cup B = B \iff A \subset B}$ 
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
#sets #subsets #union #set_equality #proof 


### A.2.1b) Show that $A \cap B = A \iff A \subset B$ 
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
#sets #subsets #intersection #set_equality #proof 


### A.2.1c) Show that $(A\cup B)\cap C = (A\cap C)\cup (B\cap C)$
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
3. Because $x\in A\cup B$ and $x\in C$, it follows that $x\in A\cap C$ or $x\in B\cap C$
By definition of the union of sets it follows that $x\in (A\cap C) \cup (B \cap C)$

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
#sets #subsets #set_equality #intersection #union #proof 


A.2.1d) 


### A.2.2a) Describe the sets $\bigcup^{N}_{n=1} \big(-\frac{1}{n},\frac{1}{n} \big)$ and $\bigcap^{N}_{n=1} \big(-\frac{1}{n},\frac{1}{n} \big)$

The union of $-\frac{1}{n}$ and $\frac{1}{n}$, starting with n=1, where $n\in \mathbb{N}$, would be the set of all rational numbers $[-1,1]$.

The intersection of $-\frac{1}{n}$ and $\frac{1}{n}$, starting with n=1, where $n\in \mathbb{N}$, would be the empty set $\emptyset$ by definition of an empty set. This is because every element in the first set, $- \frac{1}{n}$, would always be negative; yet $n=n$ for both sets. Thus these sets would never overlap because $\frac{1}{n}$ would never be negative.

#sets #intersection #union #Naturals 


### A.2.2b) Describe the sets $\bigcup^{N}_{n=1} (-n,n)$ and $\bigcap^{N}_{n=1} (-n,n)$

The union of $-n$ and $n$, starting with n=1, where $n\in \mathbb{N}$, would represent the set of $\mathbb{Z}$ by definition of the set of integers.

The intersection of $-n$ and $n$, starting with n=1, where $n\in \mathbb{N}$, would be the empty set $\emptyset$ by definition of an empty set. This is because every element in the first set, $-n$, would always be negative; yet $n=n$ for both sets. Thus these sets would never overlap because $n$ would never be negative.

#sets #intersection #union #Naturals #Integers

<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>

### A.2.2c) Describe the sets $\bigcup^{N}_{n=1} [n,n+1]$ and $\bigcap^{N}_{n=1} [n,n+1]$

The union of $n$ and $n+1$, starting with n=1, where $n\in \mathbb{N}$, would represent the set of all positive integers $\mathbb{Z}^{+}$.

The intersection of $n$ and $n+1$, starting with n=1, where $n\in \mathbb{N}$, would represent the set of all positive integers $\mathbb{Z}^{+}$. This is because every element successor in set $n$, is also an element within set $n+1$, which also includes $n$.

#sets #intersection #union #Naturals #Integers #consecutive

### A.2.3a) Describe the sets $\bigcup^{\infty}_{n=1} \big(-\frac{1}{n},\frac{1}{n} \big)$ and $\bigcap^{\infty}_{n=1} \big(-\frac{1}{n},\frac{1}{n} \big)$

The union of $-\frac{1}{n}$ and $\frac{1}{n}$, starting with n=1, where $n\in \mathbb{N}$, would be the set of all real numbers $(-\infty,\infty)$.

The intersection of $-\frac{1}{n}$ and $\frac{1}{n}$, starting with n=1,  would be the empty set $\emptyset$ by definition of an empty set. This is because every element in the first set, $- \frac{1}{n}$, would always be negative; yet $n=n$ for both sets. Thus these sets would never overlap because $\frac{1}{n}$ would never be negative.

#sets #intersection #union #Naturals 

### A.2.3b) Describe the sets $\bigcup^{\infty}_{n=1} (-n.n)$ and $\bigcap^{\infty}_{n=1} (-n,n)$

The union of $-n$ and $n$, starting with n=1, where $n\in \mathbb{N}$, would be the set of all real numbers $(-\infty,\infty)$.

The intersection of $-n$ and $n$, starting with n=1,  would be the empty set $\emptyset$ by definition of an empty set. This is because every element in the first set, $- n$, would always be negative; yet $n=n$ for both sets. Thus these sets would never overlap because $n$ would never be negative.

#sets #intersection #union #Naturals 

### A.2.3c) Describe the sets $\bigcup^{\infty}_{n=1} [n.n+1]$ and $\bigcap^{\infty}_{n=1} [n.n+1]$

The union of $n$ and $n+1$, starting with n=1, would be the set of positive real numbers $[1,\infty)$

The intersection of $n$ and $n+1$, starting with n=1,  would be the empty set $\emptyset$ by definition of an empty set. This is because every element in the second set, $n+1$, would always be 1 greater than items in the first set, n; thus these sets would never overlap because $n$ and $n+1$ would never equal.

#sets #intersection #union #Naturals 