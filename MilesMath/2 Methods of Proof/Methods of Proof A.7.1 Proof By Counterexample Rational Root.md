### Disprove the statement: For any natural number $n$ the equation $$4x^{2}+x -n=0$$ has no rational root.

To disprove this statement, a counterexample is given. 

Let's assume there is a rational root that satisfies this equation. Meaning, some number for $n$ will provide a rational root for the equation. Consider one possible root:

$x= \frac{-1+\sqrt{(1)^2-4(4)(-n)}}{2(4)}=\frac{a}{b}$

With some algebra
$$\begin{align}
\frac{-1+\sqrt{1+16n}}{8}&=\frac{a}{b}\\

-1 + \sqrt{1+16n}&=\frac{8a}{b}\\
\sqrt{1+16n}&=\frac{8a}{b}+1\\
\sqrt{1+16n}&=\frac{8a+b}{b}\\
1+16n&=\left(\frac{8a+b}{b}\right)^2\\
16n&=\left(\frac{8a+b}{b}\right)^{2}-1\\
16n&=\frac{64a^{2}+16ab +b^2}{b^{2}}-1\\
16n&=\frac{64a^{2}+16ab +b^2}{b^{2}}-\frac{b^2}{b^2}\\
16n&=\frac{64a^{2}+16ab}{b^{2}}\\
n&=\frac{64a^{2}+16ab}{16b^{2}}\\
n&=\frac{4a^2+ab}{b^{2}}\\
\end{align}$$
say a = 1 and b = 2
$$n=\frac{4(1)^2+(1)(2)}{2^2}=\frac{3}{2}$$
And so the polynomial $4x^{2}+x- \frac{3}{2}=0$ will have rational roots: $x_{1}= \frac{1}{2}$
and $x_{2} =- \frac{3}{4}$.
#irrational #rational_root #algebra_proof #counterexample