Continuity:
1. f(a) must be defined for f(x)
	- check if f(x) is defined at x=a. 
2. The $\lim_{x \to a} f(x)$ exists
	- compute $\lim_{x \to a} f(x)$ - verify that the $\lim_{x \to a^-} f(x)$ and $\lim_{x \to a^+} f(x)$ exists, then it can be said that $\lim_{x \to a} f(x)$ exists
3. The $\lim_{x \to a} f(x)=f(a)$
	- $\lim_{x \to a} f(x)$ must equal $f(a)$

Continuity on $[a,b]$:
A function $f(x)$ is said to be continuous on an interval $[a,b]$ if it is continuous at 
every number in the interval. If the limit of f(x) as x is approaching a from the right ($\lim_{x \to a^+}$) and b from the left ($\lim_{x \to b^-}$) exists, this will ensure that f(x) is continuous at every number in the interval $[a,b]$. 

We will use limit laws to show that $f(x)=3x^3+x^2-x-0.1$ is continuous on the interval $[-1,1]$. By direct substitution: 

$$\begin {align} \lim_{x \to a} f(x) &= \lim_{x \to a} 3x^3+x^2-x-0.1 \\
&=3a^3+a^2-a-0.1 \\
&=f(a)\end{align}$$
 The  Intermediate Value  Theorem  states  that  a  continuous  function  takes  on  every 
intermediate value between the function values $f(a)$ and $f(b)$. If $f(x)$  is continuous on the closed interval $[a,b]$, let N be any number between  $f(a)$ and $f(b)$, where $f(a) \ne f(b)$, there exists a number $c$ in $[a,b]$ such that $f(c)=N$. One of the implications of the Intermediate Value Theorem is that if $f(a)$ and $f(b)$ have opposite signs, then it can be said that there exists a number $c$ in $[a,b]$ such that $f(c)=0$ 

The Bisection Method requires selecting an interval of consecutive integers, and by utilizing midpoint and the implications from the Intermediate Value Theorem, find a sufficiently small enough interval on which a zero of $f(x)$ lies.

Selecting the interval $[0,1]$, and evaluating the function $f(x)=3x^3+x^2-x-0.1$ for $f(0)$ and $f(1)$, it follows that:
$$f(0)=-0.1~~~~\text{and}~~~~f(1)=2.9$$

The sign change at the interval endpoints indicates that there exists a number within the interval $[0,1]$ such that $f(c)=0$, also known as a zero or x-intercept.

The Bisection Method algorithm is as follows:
1. Evaluate the function at the interval endpoints $f(a)$ and $f(b)$
2. Find the midpoint of the interval: $mid=\dfrac{a+b}{2}$  
3. Evaluate the function at the midpoint $f(mid$)$
	- Take note of the signs. If there is a sign change between $f(a)$ and $f(b)$, then there exists a zero between (a,b). The midpoint is used to make the window smaller. The sign of f(mid) tells you which endpoint to replace, based on the corresponding sign from $f(a)$ and $f(b)$. That is, if $$ \begin{align}f(a)<0~~~&\text{and}~~~f(mid)<0 \\
	c_0=mid ~~~&\text{is the new endpoint} \\
	&[c_0,b]\end{align}$$
4. Repeat 1 - 3 with the new endpoint $c_1$, replacing endpoints based on their corresponding signs. This process should push the intervals closer and closer together until they each approximate the zero of the polynomial, approaching from the right and left hand sides. 

