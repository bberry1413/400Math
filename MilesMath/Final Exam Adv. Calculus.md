### Brandiece Berry - Advanced Calculus Final Exam - SPR 2022
__Problem 1
Show $\mathbb{Q}$ is a field with the field axioms.__
$\mathbb{Q}$ is the set of rational numbers of the form $\frac{a}{b}$ where $a\in \mathbb{Z}$ and $b\in \mathbb{N}$.

Field Axioms:
A1 - *closure under addition and commutative property of addition*: 

For any $a,b\in \mathbb{R}$ there is a number $a+b\in \mathbb{R}$ and $a+b=b+a$. 

A1 closure) Let $x,y\in\mathbb{Q}$. By definition of the set of rational numbers, 

$$x=\frac{a}{b} \hspace{0.5cm}y=\frac{c}{d}$$

where $a,c \in \mathbb{Z}$ and $b,d\in \mathbb{N}$. It is given that both $\mathbb{Z}$ and $\mathbb{N}$ are closed under addition and multiplication.  It follows that:

$$x+y=\frac{a}{b} + \frac{c}{d}$$

and with some algebra

$$\frac{ad+cb}{bd}$$

It follows that $ad,cb, ~\text{and}~ad+cb \in \mathbb{Z}$ and $bd \in \mathbb{N}$ and therefore $\frac{ad+cb}{bd} \in \mathbb{Q}$, by the definition of rational numbers. 

The addition of rational numbers creates a rational number, so $\mathbb{Q}$ is closed under addition.

A1 Commutative) 

Let $x,y\in\mathbb{Q}$. By definition of the set of rational numbers, $x=\frac{a}{b} \hspace{0.5cm}y=\frac{c}{d}$
where $a,c \in \mathbb{Z}$ and $b,d\in \mathbb{N}$. It is given that both $\mathbb{Z}$ and $\mathbb{N}$ are closed under addition and multiplication.  It follows that:

$$x+y=\frac{a}{b} + \frac{c}{d}=\frac{ad+cb}{bd}$$

and 

$$y+x=\frac{c}{d}+ \frac{a}{b}=\frac{cb+ad}{bd}$$

To verify that $x+y=y+x$,  

$$\begin{align}
\frac{ad+cb}{bd}&=\frac{cb+ad}{bd}\\
\frac{ad}{bd} + \frac{cb}{bd} &= \frac{cb}{bd} + \frac{ad}{bd}\\
\frac{a}{b}+ \frac{c}{d}&=\frac{c}{d}+ \frac{a}{b}\\
x+y &= y+x
\end{align}$$

A2 - *associative property of addition* :

For any $a,b,c\in \mathbb{R}$ the identity $(a+b)+c=a+(b+c)$ is true.

Let $x,y,z \in \mathbb{Q}$ , consider $(x+y)+z$ and given that $x=\frac{a}{b}$, $y=\frac{c}{d}$, and $z=\frac{f}{g}$ 

$$(x+y)+z=\left(\frac{a}{b} + \frac{c}{d}\right)+\frac{f}{g}$$

Using the fact that 

$$\frac{a}{b} + \frac{c}{d} = \frac{ad+cb}{bd}$$

$$\left(\frac{a}{b} + \frac{c}{d}\right)+ \frac{f}{g}=\left(\frac{ad+cb}{bd}\right)+ \frac{f}{g}=\frac{g(ad+cb)+f(bd)}{bdg}=\frac{adg+cbg+fbd}{bdg}$$

Next, consider $x+(y+z)$

$$x+(y+z)=\frac{a}{b} + \left(\frac{c}{d}+\frac{f}{g}\right)=\frac{a}{b}+ \left(\frac{cg+df}{dg}\right)=\frac{b(cg+df)+a(dg)}{bdg}=\frac{bcg+bdf+adg}{bdg}$$ 

Verify that $(x+y)+z=x+(y+z)$ 

Setting the two expressions equal to each other, simplifying, and utilizing A1:

$$\begin{align}
\frac{adg+cbg+fbd}{bdg}&=\frac{bcg+bdf+adg}{bdg}\\
\frac{adg}{bdg}+ \frac{cbg}{bdg} + \frac{fbd}{bdg} &=\frac{cgb}{bdg}+ \frac{bdf}{bdg}+ \frac{adg}{bdg}\\
\left(\frac{a}{b} + \frac{c}{d}\right)+ \frac{f}{g}&=\frac{a}{b}+ \left(\frac{c}{d}+ \frac{f}{g}\right)
\end{align}$$

It follows that $(x+y)+z=x+(y+z)$.

A3 - *existence of a zero element*:

There is a unique number $0\in \mathbb{R}$ so that, for all $a\in \mathbb{R}$, $a+0=0+a=a$.

Consider $x\in \mathbb{Q}$, where $x=\frac{a}{b}$, and $a\in \mathbb{Z}$ and $b\in \mathbb{N}$

$$x+0=\frac{a}{b}+ \frac{0}{1}=\frac{a}{b}+ \frac{0}{1}\cdot \frac{b}{b}=\frac{a+0b}{b}=\frac{a}{b}$$

A4 - *existence of a negative element* :

For any number $a\in \mathbb{R}$ there is a corresponding number denoted by $-a$ with the property that $a+(-a)=0$.

Consider $x\in \mathbb{Q}$, where $x=\frac{a}{b}$, and $a\in \mathbb{Z}$ and $b\in \mathbb{N}$

$$x+(-x)=\frac{a}{b}+(-\frac{a}{b})=\frac{a}{b}$$

Since $b\in \mathbb{N}$ it cannot be negative and so it follows

$$\frac{a}{b}+(- \frac{a}{b})=\frac{a}{b}+(\frac{-a}{b})=\frac{a-a}{b}=\frac{0}{b}=0$$

M1 - *closure under multiplication and commutative property of multiplication*:

For any $a,b\in \mathbb{R}$ there is a number $ab\in \mathbb{R}$ and $ab=ba$.

M1 Closure) Let $x,y\in\mathbb{Q}$. By definition of the set of rational numbers, 

$$x=\frac{a}{b} \hspace{0.5cm}y=\frac{c}{d}$$

where $a,c \in \mathbb{Z}$ and $b,d\in \mathbb{N}$. It is given that both $\mathbb{Z}$ and $\mathbb{N}$ are closed under addition and multiplication.  It follows that: 

$$xy=\frac{a}{b} \cdot \frac{c}{d} =\frac{ac}{bd}$$

It follows that $ac\in \mathbb{Z}$ and $bd\in \mathbb{N}$ and therefore $\frac{ac}{bd} \in \mathbb{Q}$ by the definition of rational numbers. 

The product of rational numbers creates another rational number, so $\mathbb{Q}$ is closed under multiplication

M1 Commutative Property) Consider $x\cdot y$, given that $x=\frac{a}{b}$ and $y=\frac{c}{d}$ 

$$x\cdot y = \frac{a}{b} \cdot \frac{c}{d} = \frac{ac}{bd} = \frac{ca}{db} = \frac{c}{d} \cdot \frac{a}{b} = y \cdot x$$

M2 - *associative property of multiplication*:

For any $a,b,c\in \mathbb{R}$ the identity $(ab)c=a(bc)$ is true.

Let $x,y,z \in \mathbb{Q}$ , consider$(xy)z$, given that $x=\frac{a}{b}$, $y=\frac{c}{d}$, and $z=\frac{f}{g}$. Because of M1, $xy=\frac{ac}{bd} \in \mathbb{Q}$ and it is given that $\frac{f}{g} \in \mathbb{Q}$. 

It follows that

$$(xy)z=\left(\frac{a}{b}\cdot \frac{c}{d}\right) \frac{f}{g}=\frac{acf}{bdg}=\frac{a}{b}\left(\frac{cf}{dg}\right)=\frac{a}{b}\left(\frac{c}{d} \cdot \frac{f}{g}\right)=x(yz)$$

M3 - *identity property of multiplication*:

There is a unique number $1\in \mathbb{R}$ so that $a1=1a=a$ for all $a\in \mathbb{R}$.

Consider $x\in \mathbb{Q}$, where $x=\frac{a}{b}$, and $a\in \mathbb{Z}$ and $b\in \mathbb{N}$

$$x\cdot 1=1x = 1\left(\frac{a}{b}\right)=\left(\frac{a}{b}\right)\cdot 1=\frac{a}{b}$$

M4 - *inverse property of multiplication*:

For any number $a\in \mathbb{R}, a \ne 0$, there is a corresponding number denoted $a^{-1}$ with the property that $aa^{-1}=1$.

Consider $x\in \mathbb{Q}$, where $x=\frac{a}{b}$and $a\in \mathbb{Z}$ and $b\in \mathbb{N}$

$$x\cdot x^{-1}= \frac{a}{b}\left(\frac{a}{b}\right)^{-1}$$

By the rules of exponents 

$$\left(\frac{a}{b}\right)^{-1}=\frac{b}{a}$$

It follows that 

$$\frac{a}{b}\left(\frac{a}{b}\right)^{-1}=\frac{a}{b}\left(\frac{b}{a}\right)=\frac{ab}{ba}$$ By M1 $ab = ba$ so

$$\frac{ab}{ba}=\frac{ba}{ba}=\frac{b}{b} \cdot \frac{a}{a} = 1 \cdot 1=1$$

AM1 - *distributive property*:

For any $a,b,c \in \mathbb{R}$ the identity $(a+b)c=ac+bc$ is true.

Let $x,y,z \in \mathbb{Q}$ , given that $x=\frac{a}{b}$, $y=\frac{c}{d}$, and $z=\frac{f}{g}$.  It follows that:

$$x+y=\frac{a}{b} + \frac{c}{d}=\frac{ad+cb}{bd}$$
Consider $(x+y)z$
$$\begin{align}
(x+y)z&=\left(\frac{ad+cb}{bd}\right) \frac{f}{g}\\
&=\frac{f(ad+cb)}{bdg}\\
&=\frac{adf+cbf}{bdg}\\
&=\frac{adf}{bdg}+ \frac{cbf}{bdg}
\end{align}$$
Next, consider $xz+yz$ 
$$\begin{align}
\frac{a}{b}\cdot\frac{f}{g} &+ \frac{c}{d} \cdot\frac{f}{g} \\
\frac{af}{bg}&+ \frac{cf}{dg}\\
\frac{d(af)}{bdg}&+\frac{b(cf)}{bdg}\\
\frac{adf}{bdg} &+ \frac{cbf}{bdg}
\end{align}$$
It follows that $(x+y)z=xz+yz$.
<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>

__Problem 2
Show that 

$$|x_1+x_2+...+x_{n}|\le |x_1|+|x_2|+...+|x_n|$$
__For any numbers $x_{1}, x_{2}, ...,x_{n}$__
 
Proof: 

Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true.

Basis Step: Consider $n=1$.

$|x_{1}|\le|x_{1}|~~\checkmark$

$\therefore P(1)$ is true and $1\in S$ so $S$ is not empty.

Induction Step: Assume $k\ge 1$ such that $P(k)$ is true and $k \in S$ 

$$P(k)=|x_1+x_2+...+x_{k}|\le |x_1|+|x_2|+...+|x_k|$$

$$P(k+1)=|x_1+x_2+...+x_{k}+x_{k+1}|\le |x_1|+|x_2|+...+|x_k|+|x_{k+1}|$$
By the Triangle Inequality, $|x+y|\le|x|+|y|$, 


$$P(k+1)=|x_1+x_2+...
+x_{k}+x_{k+1}|\le |x_{1}+x_{2}+...+x_{k}|+|x_{k+1}|$$

Utilizing $P(k)=|x_1+x_2+...+x_{k}|\le |x_1|+|x_2|+...+|x_k|$ gives,

$$P(k+1)=|x_1+x_2+...+x_{k}+x_{k+1}|\le |x_1|+|x_2|+...+|x_k|+|x_{k+1}|$$

Then it is shown that 

$$|x_1+x_2+...+x_{n}|\le |x_1|+|x_2|+...+|x_n|$$

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI $P(n)$ is true $\forall n \in S$.

$\$

<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>

__Problem 3
Consider the sequence defined recursively by $$x_{1}=\sqrt{2}, \hspace{0.5cm} x_{n}=\sqrt{2+x_{n-1}}$$
Show by induction that $x_{n} \le x_{n+1}$ for all $n$.__
Proof:
Let $S\subset \mathbb{N}$ such that $\forall n \in S$, $P(n)$ is true.
Basis Step: Consider $n=1$
$$\begin{align}
x_{1}&<x_{2}\\
\sqrt{2}&<\sqrt{2+\sqrt{2}}\\
1.414&<1.847 ~~\checkmark
\end{align}$$

$\therefore P(1)$ is true and $1\in S$ so $S$ is not empty.
Induction Step: Assume $k\ge 1$ such that $P(k)$ is true and $k \in S$
Consider $x_{k}<x_{k+1}$ , with some algebra
$$\begin{align}
x_{k}&<x_{k+1}\\
+2~&~~+2\\
2+x_{k}&<2+x_{k+1}\\
\sqrt{2+x_{k}}&<\sqrt{2+x_{k+1}}\\
\text{Hence,}~~~~x_{k+1}&<x_{k+2}
\end{align}$$

So, $P(k)\Rightarrow P(k+1)$ and $S=\mathbb{N}$. 

$\therefore$ By PMI for $x_{1}=\sqrt{2}, x_{n}=\sqrt{2+x_{n-1}}~~~\forall n\in \mathbb{N}$, $x_{n}\le x_{n+1}$.
$\blacksquare$

<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>

__Problem 4
If $\{s_{n}\}$ is a sequence of positive number converging to 0, show that $\{\sqrt{s_{n}}\}$ also converges to zero.__

Let $\epsilon>0$. Since ${s_n}$ is convergent, we can find an $N \in \mathbb{N}$ such that $\forall n>N$, $$|s_{n}|<\epsilon^2$$
Since $s_{n}>0, |s_{n}|=s_{n}$
Therefore $s_{n}<\epsilon^2$
With some algebra
$$\begin{align}
s_{n}&<\epsilon^{2}\\
\sqrt{s_{n}}&<\sqrt{\epsilon^2}\\
|\sqrt{s_n}-0|&<\epsilon
\end{align}$$
$\blacksquare$

<div style="page-break-after: always; visibility: hidden"> \pagebreak </div>

__Problem 5
Which statements are true?__
	1. If $\{s_{n}\}$ and $\{t_{n}\}$ are both divergent then so is $\{s_{n}+t_{n}\}$. True
	2. If $\{s_{n}\}$ and $\{t_{n}\}$ are both divergent then so is $\{s_{n}t_{n}\}$. True
	3. If $\{s_{n}\}$ and $\{s_{n}+t_{n}\}$ are both convergent then so is $\{t_{n}\}$. False
	4. If $\{s_{n}\}$ and $\{s_{n}t_{n}\}$ are both convergent then so is $\{t_{n}\}$. True
	5. If $\{s_{n}\}$ convergent then so too is $\{\frac{1}{s_{n}}\}$. True
	6. If $\{s_{n}\}$ convergent then so too is $\{(s_{n})^2\}$.  True
	7. If $\{(s_{n})^2\}$convergent then so too is  $\{s_{n}\}$. False
