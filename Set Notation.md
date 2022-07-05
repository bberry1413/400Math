### Appendix A.2.1 - Set Notation and Vocabulary
#ElementaryRealAnalysisNotes
- __Set__: a well defined collection of items
	- __element__: an item in a set, given by $x \in A$, as in "x is an element of set A"
- __Subset__: If A and B are sets, the A is a subset of B, given by $A \subset B$, iff every element of A is also an element of B. $$ A \subset B =\forall x,~\text{if}~ x \in A, \text{then}~ x \in B $$
	- If $A \not\subset B$ then at least one element of A that is not an element of B.
- __Union__:  the set containing elements of either set A or B. $$A \cup B = \forall x, x \in A~\text{or}~x\in B ~\text{or}~x \in \text{both A \& B}$$
	- If $A \cup B$ exists, then x must be an element of set A or B or $A \cap B$ 
![[Union sets.png|250]]
- __Intersection__: the set containing elements from set A and set B $$A \cap B = \forall x, x \in \text{both A or B}$$
	- If $A \cap B$ exists, x must be an element of BOTH A and B in order to be $x \in A \cap B$ 
![[intersection sets.png|300]]
- __Difference__: the set consisting of elements that belong to A only, with respect to B $$\begin{align}A \setminus B &= \forall x,~x \in A~\text{less}~B\\ A \setminus B &= \forall x, x \in A ~\text{and}~ x \not\in B \end{align}$$
	- If $A \setminus B$ exists, x must be an element of A and NOT B
![[difference sets.png|250]]

