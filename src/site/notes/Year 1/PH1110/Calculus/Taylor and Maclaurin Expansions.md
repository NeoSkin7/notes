---
{"dg-publish":true,"permalink":"/year-1/ph-1110/calculus/taylor-and-maclaurin-expansions/","dg-note-properties":{}}
---

Some standard Maclaurin expansions are:
$$
\begin{alignat*}{2}
\sin{x}=&x-\frac{x^3}{3!}+\frac{x^5}{5!}-\frac{x^7}{7!}+\cdots+\left(-1\right)^n\frac{x^{2n+1}}{\left(2n+1\right)!}+\cdots&&=\sum^{\infty}_{n=0}{\left(-1\right)^n\frac{x^{2n+1}}{\left(2n+1\right)!}}\\\cos{x}=&1-\frac{x^2}{2!}+\frac{x^4}{4!}-\frac{x^6}{6!}+\cdots+\left(-1\right)^n\frac{x^{2n}}{\left(2n\right)!}+\cdots&&=\sum^{\infty}_{n=0}{\left(-1\right)^n\frac{x^{2n}}{\left(2n\right)!}}\\e^x=&1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+\frac{x^4}{4!}+\frac{x^5}{5!}+\cdots+\frac{x^n}{n!}+\cdots&&=\sum^{\infty}_{n=0}{\frac{x^{n}}{n!}}\\\ln{\left(1+x\right)}=&x-\frac{x^2}{2}+\frac{x^3}{3}-\frac{x^4}{4}+\frac{x^5}{5}+\cdots+\left(-1\right)^n\frac{x^n}{n}+\cdots&&=\sum^{\infty}_{n=1}{\left(-1\right)^n\frac{x^n}{n}}\\
\left(1+x\right)^p=&1+px+\frac{p(p-1)x^2}{2!}+\cdots+\frac{p!x^n}{n!\left(p-n\right)!}+\cdots&&=\sum^{p}_{n=0}{\frac{p!x^n}{n!\left(p-n\right)!}}
\end{alignat*}
$$
These can be calculated using the Taylor expansion method at $x=0$.
# Taylor Expansion
The Taylor expansion of the function $f(x)$ about $x=a$ has the following form:
$$
f(x)|_{x=a}=f(a)+f^{\prime}(a)(x-a)+\frac{f^{\prime\prime}(a)}{2!}(x-a)^2+\cdots+\frac{f^{(n)}(a)}{n!}(x-a)^n+\cdots
$$
# Maclaurin Expansion
As the Maclaurin expansion is a Taylor expansion about $x=0$, it can be written in the following form:
$$
f(x)|_{x=0}=f(0)+f^{\prime}(0)x+\frac{f^{\prime\prime}(0)}{2!}x^2+\cdots+\frac{f^{(n)}(0)}{n!}x^n+\cdots
$$
# Euler’s Formula
From the Maclaurin expansions of $\sin{x}$ and $\cos{x}$ and by considering the $e^x$ expansion, an expression for $e^{ix}$ can be obtained:
$$
e^{ix}=\cos{x}+i\sin{x}
$$
This is Euler’s Formula. A generalised form of this is:
$$
Ae^{i\alpha x}=A\left[\cos{\alpha x}+i\sin{\alpha x}\right]
$$
which forms the basis of complex numbers:
$$
z=a+bi=re^{i\varphi}=r\left[\cos{\varphi}+i\sin{\varphi}\right]
$$