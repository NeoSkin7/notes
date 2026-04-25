---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/ordinary-differential-equations-od-es/","dg-note-properties":{}}
---

An $n$th order differential equation has $n$ linearly independent solutions and $n$ arbitrary constants for the general solution.
To solve for the arbitrary constants, $n$ boundary conditions are required.
# First Order
## Separable
$$
\text{General form: }\frac{\mathrm{d}y}{\mathrm{d}x}=f(x)g(y)\\
\implies \frac{1}{g(y)}\frac{\mathrm{d}y}{\mathrm{d}x}=f(x)\\
\therefore \int{\frac{1}{g(y)}}\,\mathrm{d}y=\int{f(x)}\,\mathrm{d}x
$$
## Almost Separable
$$
\text{General form: }\frac{\mathrm{d}y}{\mathrm{d}x}=f(ax+by)\\
\text{Let }z=ax+by\\
\therefore \frac{\mathrm{d}z}{\mathrm{d}x}=a+b\frac{\mathrm{d}y}{\mathrm{d}x}\\
\implies \frac{\mathrm{d}z}{\mathrm{d}x}=bf(z)+a\\
\therefore \int{\frac{1}{bf(z)+a}\,\mathrm{d}z}=\int{1}\,\mathrm{d}x\\
\text{Then substitute }z=ax+by
$$
## Homogeneous
Homogeneous equations have the form:
$$
f(tx,ty)=t^nf(x,y)
$$
For these types of differential equations, attempt a substitution of $y=vx$, such that $v=\frac{y}{x}$. A rearrangement of the equations will allow for this substitution.
## Almost Homogeneous
For equations which are homogeneous except for constants, e.g.:
$$
\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{y+x-5}{y-3x-1}
$$
attempt a substitution with $\bar{y}=y+a$ and $\bar{x}=x+b$, where suitable choices for the variables $a$ and $b$ yields:
$$
\frac{\mathrm{d}\bar{y}}{\mathrm{d}\bar{x}}=\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{\bar{y}+\bar{x}}{\bar{y}-3\bar{x}}\\
\implies \frac{\mathrm{d}y}{\mathrm{d}x}=\frac{\frac{\bar{y}}{\bar{x}}+1}{\frac{\bar{y}}{\bar{x}}-3}
$$
which is solvable via a substitution of $v=\frac{\bar{y}}{\bar{x}}$ as above.
## Common Derivative
$$
\text{General form: }f(x)\frac{\mathrm{d}y}{\mathrm{d}x}+\frac{\mathrm{d}f(x)}{\mathrm{d}x}y=Q(x)\\
\implies\frac{\mathrm{d}}{\mathrm{d}x}f(x)y=Q(x)\\
\therefore f(x)y=\int{Q(x)}\,\mathrm{d}x
$$
## Integrating Factor
$$
\text{General form: }f(x)\frac{\mathrm{d}y}{\mathrm{d}x}+P(x)y=Q(x)\\
\implies \frac{\mathrm{d}y}{\mathrm{d}x}+\frac{P(x)}{f(x)}y=\frac{Q(x)}{f(x)}\\
\text{Let }\mu(x)=\exp{\int{\frac{P(x)}{f(x)}}\,\mathrm{d}x}\\
\therefore \mu(x)\frac{\mathrm{d}y}{\mathrm{d}x}+\mu(x)\frac{P(x)}{f(x)}y=\mu(x)\frac{Q(x)}{f(x)}\\
\implies \frac{\mathrm{d}}{\mathrm{d}x}\mu(x)y=\mu(x)\frac{Q(x)}{f(x)}\\
\therefore \mu(x)y=\int{\mu(x)\frac{Q(x)}{f(x)}}\,\mathrm{d}x
$$
where $\mu(x)$ is the integrating factor.
## Bernoulli Equation
$$
\text{General form: }\frac{\mathrm{d}y}{\mathrm{d}x}+P(x)y=Q(x)y^n\\
\text{Let }z=y^{1-n}\\
\implies \frac{\mathrm{d}z}{\mathrm{d}x}=(1-n)y^{-n}\frac{\mathrm{d}y}{\mathrm{d}x}\\
\therefore \frac{\mathrm{d}z}{\mathrm{d}x}+P(x)(1-n)z=(1-n)Q(x)\\
$$
This rearrangement matches the form required for an integrating factor method.
# Second Order
## Homogeneous
$$
\text{General form: }a\frac{\mathrm{d}^2y}{\mathrm{d}x^2}+b\frac{\mathrm{d}y}{\mathrm{d}x}+cy=0\\
\text{All solutions of the form }y=e^{mx}\\
\therefore am^2e^{mx}+bme^{mx}+ce^{mx}=0\\
\implies am^2+bm+c=0\\
\therefore m_\pm=\frac{-b\pm\sqrt{b^2-4ac}}{2a}\\
\implies y=Ae^{m_+x}+Be^{m_-x}
$$
### Complex Roots
$$
\text{General solution: }y=Ce^{(p+iq)x}+De^{(p-iq)x}\\
\implies y=e^{px}\left[Ce^{iqx}+De^{-iqx}\right]=e^{px}\left[(C+D)\cos{qx+i(C-D)\sin{qx}}\right]\\
\therefore y=e^{px}\left[A\cos{qx}+B\sin{qx}\right]
$$
### Equal Roots
$$
\text{General solution: }y=Ae^{mx}\text{ where $m$ is a doubled root}\\
y=Bxe^{mx}\text{ is also a solution}\\
\therefore y=(A+Bx)e^{mx}
$$
This solution is found as $y=e^{mx}$ is multiplied by a function $v=A+Bx$ which goes to zero under a second derivative and therefore also leads to a correct result of the ODE equalling zero.
## Non-Homogeneous
$$
\text{General form: }a\frac{\mathrm{d}^2y}{\mathrm{d}x^2}+b\frac{\mathrm{d}y}{\mathrm{d}x}+cy=f(x)\\
\implies\left(aD_x^2+bD_x+c\right)y=f(x)\\
\therefore(D_x+\alpha)(D_x+\beta)y=f(x)\text{ for roots $\alpha$ and $\beta$}\\
\text{Let }u=(D_x+\beta)y\\
\implies (D_x+\alpha)u=f(x)\iff\frac{\mathrm{d}u}{\mathrm{d}x}+\alpha u=f(x)\\
\text{Which is first order -- solve and substitute $u$:}\\
(D_x+\beta)y=u\\
\text{Which is also first order -- solve for final solution}
$$
Note that $D_x$ is the differential operator, defined as:
$$
D_x\,f(x)=\frac{\mathrm{d}}{\mathrm{d}x}f(x)
$$
> [!note] ✏️
> This notation is used for simplicity within the above equations, but is not taught in the course. A general approach for solving non-homogeneous second-order linear differential equations is outlined using [The Method of Undetermined Coefficients](/2ce052c19808802e8e85d25923ee84a4#2d1052c19808801d9a6fc3fde66aafae), and is the preferred method for the course.

### Trigonometric Functions
When $f(x)$ is a trigonometric function $A\sin{\alpha x}$ or $A\cos{\alpha x}$, recall:
$$
Ae^{i\alpha x}=A\left[\cos{\alpha x}+\sin{\alpha x}\right]
$$
So the following equation could instead be solved:
$$
a\frac{\mathrm{d}^2Y}{\mathrm{d}x^2}+b\frac{\mathrm{d}Y}{\mathrm{d}x}+cY=Ae^{i\alpha x}
$$
and the real or imaginary part of the solution taken dependent on the function:
$$
f(x)=\begin{cases}
A\cos{\alpha x}\implies y=\Re{(Y)}\\
A\sin{\alpha x}\implies y=\Im{(Y)}
\end{cases}
$$
### Sums of Functions
When $f(x)$ is the sum of functions, the ODE can be broken into a series of component ODEs:
$$
a\frac{\mathrm{d}^2y}{\mathrm{d}x^2}+b\frac{\mathrm{d}y}{\mathrm{d}x}+cy=f_1(x)+f_2(x)+\cdots\implies\begin{cases}
a\frac{\mathrm{d}^2y}{\mathrm{d}x^2}+b\frac{\mathrm{d}y}{\mathrm{d}x}+cy=f_1(x)\\
a\frac{\mathrm{d}^2y}{\mathrm{d}x^2}+b\frac{\mathrm{d}y}{\mathrm{d}x}+cy=f_2(x)\\
\hspace{5em} \vdots
\end{cases}
$$
The solutions to these component ODEs can then be added together for the solution to the sum ODE:
$$
y=y_1+y_2+\cdots
$$
### The Method of Undetermined Coefficients
If you know the required solution form for an ODE equal to a function $f(x)$, you can instead substitute the solution form and solve for unknown coefficients using algebra. The standard trial solutions are outlined below.
This gives the particular solution $y_p$, but adding a term that differentiates to zero does not change the behaviour of the ODE, so we must add the solution of the homogeneous version, $y_c$, which is given by the complementary function:
$$
a\frac{\mathrm{d}^2y_c}{\mathrm{d}x^2}+b\frac{\mathrm{d}y_c}{\mathrm{d}x}+cy_c=0
$$
Giving the full solution:
$$
y=y_c+y_p
$$
**Trial Solutions**
$$
f(x)=
\begin{cases}
Ce^{kx}&\implies y_p=\begin{cases}Axe^{kx},&\text{ if $Ae^{kx}$ in $y_c$}\\Ax^2e^{kx},&\text{ if $Axe^{kx}$ in $y_c$}\\
Ae^{kx},&\text{otherwise}
\end{cases}\\
c_0+c_2x+c_3x^2+\cdots+c_nx^n&\implies y_p=A_0+A_1x+A_2x^2+\cdots+A_{n+2}x^{n+2}\\
C\cos{\alpha x}\text{ or }C\sin{\alpha x}&\implies y_p=A\cos{\alpha x}+B\sin{\alpha x}\\
Ce^{kx}\cos{\alpha x}\text{ or }Ce^{kx}\sin{\alpha x}&\implies y_p=e^{kx}\left(A\cos{\alpha x}+B\sin{\alpha x}\right)
\end{cases}
$$