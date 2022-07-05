## Cramer's Rule 
#### (Applications of the Determinant)
If a system of linear eq in $n$ variables has a coefficient matrix $A$ with a nonzero $\det(A)$ the solution to the system is:

$x_1=\dfrac{\det(A_1)}{\det(A)}$,  $x_2=\dfrac{\det(A_2)}{\det(A)}, \ldots,x_n=\dfrac{\det(A_n)}{\det(A)}$

Where the $ith$ column of $A_i$ is the column in the system of equations $Ax=b$

__EX] Consider the system of eq:__  

$$\begin{align}
  x+3y&=5\\
  2x-5y&=7
\end{align}$$

can also be written as: $Ax=b$ => 
$$\begin{align}
  1&~3\\
  2&-5
\end{align}$$ 
\[\begin{align}
  x\\
  y
\end{align}\]=\[\begin{align}
  5\\
  7
\end{align}\]$$ where A is the coefficient matrix:

$A$ = $\left[\begin{align}
  1&3\\
  2&-5
\end{align}\right]$ 
- If we replace the 1st column with the b column of the solution matrix it gives: 
$A_1$ = $\left[\begin{align}
  5&3\\
  7&-5
\end{align}\right]$
- If we replace the 2nd column with the b column of the solution matrix it gives:
$A_2$ = $\left[\begin{align}
  1&5\\
  2&7
\end{align}\right]$$ 



$$\left[\begin{array}{}
 1&4\\
 -1&4
\end{array}\right]\hspace{4cm} \left[\begin{array}{}
 1&2&3\\
 4&5&6\\
 7&8&9
\end{array}\right]$$