## Cramer's Rule 
#### (Applications of the Determinant)
If a system of linear eq in $n$ variables has a coefficient matrix $A$ with a nonzero $\det(A)$ the solution to the system is:

$x_1=\dfrac{\det(A_1)}{\det(A)}$,  $x_2=\dfrac{\det(A_2)}{\det(A)}, \ldots,x_n=\dfrac{\det(A_n)}{\det(A)}$

Where the $ith$ column of $A_i$ is the column in the system of equations $Ax=b$

__EX] Consider the system of eq:__  
$\begin{array}{cc}
  x+3y&=&5\\
  2x-5y&=&7
\end{array}$

can also be written as: 
$Ax=b$ => $\left[\begin{array}{cc}
  1&3\\
  2&-5
\end{array}\right] \left[\begin{array}{cc}
  x\\
  y
\end{array}\right]=\left[\begin{array}{cc}
  5\\
  7
\end{array}\right]$ where A is the coefficient matrix:

$A$ = $\left[\begin{array}{cc}
  1&3\\
  2&-5
\end{array}\right]$ 
- If we replace the 1st column with the b column of the solution matrix it gives: 
$A_1$ = $\left[\begin{array}{cc}
  5&3\\
  7&-5
\end{array}\right]$
- If we replace the 2nd column with the b column of the solution matrix it gives:
$A_2$ = $\left[\begin{array}{cc}
  1&5\\
  2&7
\end{array}\right]$ 
