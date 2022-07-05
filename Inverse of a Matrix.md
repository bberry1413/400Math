## The Inverse of a Matrix

__Def]__ An $n\times n$ matrix $A$ is __invertible/nonsingular__ when there exists an $n \times n$ matrix $B$ such that: $$AB = BA = I_n$$
where $I_n$ is the identity matrix of order $n$. The matrix $B$ is the multiplicative inverse of $A$. 
- A matrix that does not have an inverse is __noninvertible/singular__

__Theorem 2.7]__ If $A$ is an invertible matrix, then it's inverse is unique. The inverse of A is denoted by $A^{-1}$

__EX]__ Show that $B$ is the inverse of $A$ where:
$A$ = $\left[\begin{array}{cc}
  -1&2\\
  -1&1
\end{array}\right]$ and  $B$ = $\left[\begin{array}{cc}
  1&-2\\
  1&-1
\end{array}\right]$ 

If $B$ is an inverse of $A$ then $$AB = I$$

$\therefore$
$AB$ = $\left[\begin{array}{cc}
  \color{red}-1&\color{red}2\\
  \color{orange}-1&\color{orange}1
\end{array}\right]$  $\left[\begin{array}{cc}
  \color{green}1&\color{cyan}-2\\
  \color{green}1&\color{cyan}-1
\end{array}\right]$

- _using row x column, the product of a 2x2 and a 2x2 should be a 2x2_

$\small{headwork, PS = \text{Product \& Sum}}$
$~~~~~~~~~\small{PS1}~~~~~~~~~~~~~~~~~~~~~~PS2$
$\color{red}-1\color{green}(1)$ + $\color{red}2\color{green}(1) ~ ~ ~ ~\color{red}-1\color{cyan}(-2)$ + $\color{red}2\color{cyan}(-1)$
$\color{orange}-1$$(1)$ + $\color{orange}1$$(1)~ ~ ~ ~$ $\color{orange}-1$$(-2)$ + $\color{orange}1$$(-1)$

$AB$ = $\left[\begin{array}{cc}
  -1+2&2-2\\
  -1+1&2-1
\end{array}\right] =  \left[\begin{array}{cc}
  1&0\\
  0&1
\end{array}\right] = I$    

__EX]__ Find the inverse of: $A$ = $\left[\begin{array}{cc}
  1&4\\
  -1&-3
\end{array}\right]$ 

- _1st way to find the inverse of a matrix: Gauss Jordan Elimination_
$[A~~\vdots~~I]$ => $[I~~\vdots~~A^{-1}]$ w/ Gauss/Jordan

$= \left[\begin{array}{cccc}
  1&4&\vdots~~1&0\\
  -1&-3&\vdots~~0&1
\end{array}\right]$  $R_2+R_1 \rightarrow R_2 ~~ (\small{headwork})$   $\begin{array}{ccccc}
  &1&4&1&0\\
  +&-1&-3&0&1\\
  \hline\
  &0&1&1&1
\end{array}$

$= \left[\begin{array}{cccc}
  1&4&1&0\\
  0&1&1&1
\end{array}\right]$  $-4R_2+R_1 \rightarrow R_1~~(\small{headwork})$   $\begin{array}{ccccc}
  -4&(0&1&1&1)\\
  +&1&4&1&0
\end{array} =\begin{array}{ccccc}
  &0&-4&-4&-4\\
  +&1&4&1&0\\
 \hline \
 R_1&1&0&-3&-4
\end{array}$

$= \left[\begin{array}{cccc}
  1&0&-3&4\\
  0&1&1&1
\end{array}\right]$ 

__EX]__ Find the inverse of:  $A = \left[\begin{array}{ccc}
 1&-1&0\\
  1&0&-1\\
  -6&2&3
  \end{array}\right]$

$AI=\left[\begin{array}{cccccc}
  1&-1&0&\vdots~~1&0&0\\
  \color{red}1&0&-1&\vdots~~0&1&0\\
  -6&2&3&\vdots~~ 0&0&1\\
\end{array}\right]$ $-R_2+R_1 \rightarrow R_2 ~~\small{(headwork)}$ $=\begin{array}{ccccccc}
  -1&(1&0&-1&0&1&0)\\
  +&1&-1&0&1&0&0\\
 \hline \
 R_2&0&-1&1&1&-1&0
\end{array}$

$=\left[\begin{array}{cccccc}
1&-1&0&1&0&0\\
0&-1&1&1&-1&0\\
\color{red}-6&2&3&0&0&1
\end{array}\right]$ $6R_1+R_3 \rightarrow R_3$ 
$\small{(headwork)}$
$=\begin{array}{ccccccc}
  6&(1&-1&0&1&0&0)\\
  +&-6&2&3&0&0&1\\
\end{array}$ $=\begin{array}{ccccccc}
  &6&-6&0&6&0&0\\
  +&-6&2&3&0&0&1\\
 \hline \
 R_3&0&-4&3&6&0&1
\end{array}$ $\rightarrow\left[\begin{array}{cccccc}
1&-1&0&1&0&0\\
0&-1&1&1&-1&0\\
0&-4&3&6&0&1
\end{array}\right]$ 

$-R_2 \rightarrow R_2$ $\rightarrow\left[\begin{array}{cccccc}
1&-1&0&1&0&0\\
0&1&-1&-1&1&0\\
0&-4&3&6&0&1
\end{array}\right]$ $4R_2+R_3 \rightarrow R_3 ~~ \small{(headwork)}
$ $=\begin{array}{ccccccc}
  4&(1&-1&0&1&0&0)\\
  +&0&-4&3&6&0&1\\
\end{array}$ $=\begin{array}{ccccccc}
  &4&--4&0&4&0&0\\
  +&-6&2&3&0&0&1\\
 \hline \
 R_3&0&-4&3&6&0&1
\end{array}$