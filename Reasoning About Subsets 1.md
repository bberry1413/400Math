### Guide to Proofs on Sets
_Stanford CS103 pdf_
#Sets, #Subsets, #Proofs 
[[Set Notation]]
[[Proofs Practice 1 - Sets]]

EX] Prove the theorem: For any sets A, B, C, D, and E where $A \subset B \cup C,~B \subset D,~\text{and}~C \subset E$  we have $A \subset D \cup E$ 

Steps to prove $A \subset D \cup E$ :
1. Start with the __GIVEN__ statement: 
- __For any sets A, B, C, D, and E where $\mathbf{A \subset B \cup C,~B \subset D,~\text{and}~C \subset E}$__
2. To prove $A \subset B \cup C$ we must pick an arbitrary element $x \in A$ and show that it is also within $D \cup E$
- We need to use the implications of the __GIVEN__
	1. If you know that $x \in A$ and $A \subset B \cup C$, by the definition of subsets, we can conclude that $x \in B \cup C$ 
	2. 