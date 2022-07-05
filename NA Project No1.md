## NA Project 1: Floating Point Conversion
### MA 441 - Numerical Analysis - Brandiece Berry
#### Instructions
Convert your number __7.7__ 
1. A double precision format
2. Round to proper rounding rule
3. Find the absolute error
4. Find the relative error
5. Do an error analysis to show that your conversion is within machine epsilon error
6. Write up your results. Be sure to describe the process for each step.
#### Decimal to Binary
We can represent a decimal number as $$…+a_2\times 10^2+a_1\times 10^1+a_0\times 10^0.b_0\times 10^{-1}+b_1\times 10^{-2}+b_2\times 10^{-3}+…$$ where the $a_{n}$ terms represent the whole number portion and the $b_{n}$terms represent the fractional portion, which is either given as a terminating or repeating decimal. 

Binary numbers can be represented by $$…+a_{2*}\times 2^2+a_{1*}\times 2^1+a_{0*}\times 2^0.b_{0*}\times 2^{-1}+b_{1*}\times 2^{-2}+b_{2*}\times 2^{-3}+…$$ where the $a_{n*}$ terms represent the base 10 equivalent binary digit or bit for each place and the $b_{n*}$ terms represent the equivalent fractional portion of the base 10 number in binary.  

 The first step in converting a decimal to it's equivalent binary form is to split the number into two parts, it's whole number and decimal portions. Whole numbers can be easily converted into binary through the following algorithm: divide by 2, keep the resulting quotient and record the corresponding remainder, which becomes the new binary digit for that place. Repeat dividing by 2 with the previous quotient and record the remainder until the resulting quotient is 0. 
 $$\begin{align} 
2 &|7=&1~~~\\
2 &|3=&1~~~\\
2 &|1=&1~~~&~~~\text{<Binary Starts Here}\uparrow\\
2 &|0&~~~\text{STOP}
\end{align}$$
The decimal portion can be converted using the following algorithm: multiply by 2, if the resulting product is $\ge 1$, record a 1 as the new binary digit for that place. Next, if the product is $\ge 1$, keep the decimal portion as the next product to perform in the algorithm. That is, if $2\times (0.b_0)=1.b_1$ , we record a 1 as that place's binary digit. Then the next multiplication will be $2 \times (0.b_1)$ and so on. However, if the product is $<1$, that is, if $2\times (0.b_0)=0.b_1$, record a 0 as that place’s binary digit and perform $2 \times (0.b_1)$. Repeat this multiplication and selection procedure with the new decimal part, $b_1$ until the decimal terminates or forms a repeating pattern. 
$$\begin{align}
2 \times 0.7 &= 1.4 \rightarrow 1&\text{<Binary Starts Here \downarrow}\\
2 \times 0.4 &= 0.8 \rightarrow 0 \\
2 \times 0.8 &= 1.6 \rightarrow 1 \\
2 \times 0.6 &= 1.2 \rightarrow 1 \\
2 \times 0.2 &= 0.4 \rightarrow \underline{0} \\
2 \times 0.4 &= 0.8 \rightarrow 0& \text{STOP, repeating}~\overline{0110}\downarrow
\end{align}$$

Here, the algorithm stops at the 5th place because after, in the 6th place, the digits follow the same pattern as previous, $011001100110…$.

Therefore,  $(7.7)_{10}=(111.1\overline{0110})_2$

#### IEEE Double Precision Floating Point Number
In order to write $111.1\overline{0110}$ in double precision format, we need to normalize the binary form and write it as a product of $2^n$, where n represents a bit place in the binary digit. Normalizing requires moving the decimal in the binary format to the left until the remaining leftmost bit is 1. 
$$111.1\overline{0110} \rightarrow 1.111\overline{0110} \times 2^2$$

#### The Round to the Nearest Rule
Next, we write the 52 bit mantissa for the number in order to select the proper Round to the Nearest Rule.

$$+1.[11101100110011001100110011001100110011001100110011001100]110… \times2^2$$

Since the 53rd bit is a 1, and there aren’t trailing 0’s after the 53rd 1, the double precision format of $111.1\overline{0110}$ is: $$+1.[11101100110011001100110011001100110011001100110011001101 \times2^2$$
#### Rounding Error
We arrived at the floating point representation by discarding the infinte tail $$\overline{.1100}\times 2^{-52} \times 2^{2}=\overline{.0110}\times 2^{-51} \times 2^2$$ from the tail end of the number then adding $2^{-52} \times 2^2$ or $2^{-50}$ in the rounding step. We must account for this “chopping” during the analysis of the error that was introduced by the Round to the Nearest rule to ensure our value is within the IEEE machine arithmetic model of $\dfrac{1}{2} \epsilon_{mach}$.

Converting the chopped portion $\overline{.0110}\times 2^{-51} \times 2^2$  to decimal form requires a similar chopping procedure that converts the repeating binary to it’s equivalent fractional form. Moving the binary decimal to the left to find a decimal equivalent version of the repeating binary gives:
$$\begin{align}
x &= 0.\overline{0110}\\
2^4x &=0110.\overline{0110}\\
2^4x-x&= 0110.\overline{0110} - 0.\overline{0110} \\
16x-x &=0110~~~~<(110)_2 = 1\cdot 2^2+1 \cdot 2^1+0 \cdot 2^0 = (6)_{10}\\
15x & = 6\\
x &= \frac{6}{15}=0.4
\end{align}$$
So it follows that $$0.\overline{0110} \times 2^{-51} \times 2^2=0.4 \times 2^{-51} \times 2^2$$ Simplifying gives $$=0.4 \times 2^{-49}$$
#### Absolute Error
The IEEE double precision floating point number associated with 7.7 is given by $fl(7.7)$:
$$\begin{align}
fl(7.7) &= 7.7 + 2^{-50}-0.4 \times 2^{-49} \\
 &= 7.7 + (2^{-50}-0.4 \times 2^{-49}) \\
 &= 7.7 + (1-0.4 \times 2^{1}) \cdot 2^{-50} \\
 &= 7.7 + (1-0.8) \cdot 2^{-50} \\
 &= 7.7 + (0.2) \cdot 2^{-50}
\end{align}$$
Where $0.2 \times 2^{-50}$ is the absolute error, or the error introduced from the Round to the Nearest Rule. 
#### Relative Error
Now we must check if the relative error is within the IEEE machine arithmetic model of no more than $\dfrac{1}{2} \epsilon_{mach}$ or $\dfrac{1}{2} \cdot 2^{-52}$. The formula is given by: $$\dfrac{|fl(x)-x|}{|x|} \le \dfrac{1}{2} \epsilon_{mach}$$ where $|fl(x)-x|$ is the absolute error and x is the original base 10 number. 
#### Error Analysis
For $(7.7)_{10}$ it follows:
$$\dfrac{0.2 \times 2^{-50}}{7.7} \le \dfrac{1}{2} \epsilon_{mach} $$

In order to check the validity of this statement, we need to rewrite $\dfrac{0.2 \times 2^{-50}}{7.7}$ as a single fraction. Firstly, let us attempt to simplify. This is easily accomplished by multiplying the numerator and denominator by 10. It is clear that there are no other common factors and 
$$\begin{align}
\dfrac{10}{10}\cdot \dfrac{0.2 \times 2^{-50}}{7.7} &\le \dfrac{1}{2} \epsilon_{mach}\\
\dfrac{2 \times 2^{-50}}{77} &\le \dfrac{1}{2} \epsilon_{mach}\\
\end{align}$$

Next, in order to compare  $\dfrac{2 \times 2^{-50}}{77}$ to $\dfrac{1}{2} \epsilon_{mach} = \dfrac{1}{2} \cdot 2^{-52}$ we must multiply by powers of 2 until we have the base 2 exponents are equal. For this scenario, we need to combine the numerator to a single power of 2: $$\dfrac{2^1 \times 2^{-50}}{77}=\dfrac{2^{-49}}{77}$$
and multiply by a power of 2 that will create a $2^{-52}$ within our error:
 $$\dfrac{2^{-49}}{77}\cdot \dfrac{2^{-3}}{2^{-3}}=\dfrac{2^3 \times 2^{-52}}{77}=\dfrac{8}{77}\cdot 2^{-52}$$

Finally, we compare our error to $\dfrac{1}{2} \epsilon_{mach}$ or $\dfrac{1}{2} \cdot 2^{-52}$. 

It follows that:
$$\dfrac{8}{77}\cdot 2^{-52} \le \dfrac{1}{2} \epsilon_{mach}$$ is true. 