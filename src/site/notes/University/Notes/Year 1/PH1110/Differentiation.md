---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/differentiation/","dg-note-properties":{}}
---

# Definition from First Principles
$$
\frac{\mathrm{d}}{\mathrm{d}x}f(x)=\lim_{\Delta x\to0}{\left[\frac{f(x+\Delta x)-f(x)}{\Delta x}\right]}
$$
# Rules
From the first principles definition, a number of differentiation rules can be derived.
## Product Rule
$$
\text{for a function } y=f(x)=u(x)\cdot v(x),\\
\begin{align*}
\frac{\mathrm{d}y}{\mathrm{d}x}&=\lim_{\Delta x\to0}{\left[\frac{u(x+\Delta x)\cdot v(x+\Delta x)-u(x)\cdot v(x)}{\Delta x}\right]}\\
&=\lim_{\Delta x\to0}{\left[\frac{u(x+\Delta x)\left[v(x+\Delta x)-v(x)\right]+v(x)\left[u(x+\Delta x)-u(x)\right]}{\Delta x}\right]}\\
&=\lim_{\Delta x\to0}{\left[u(x+\Delta x)\frac{v(x+\Delta x)-v(x)}{\Delta x}\right]}+\lim_{\Delta x\to0}{\left[v(x)\frac{u(x+\Delta x)-u(x)}{\Delta x}\right]}\\
&=u(x)\frac{\mathrm{d}v(x)}{\mathrm{d}x}+v(x)\frac{\mathrm{d}u(x)}{\mathrm{d}x}
\end{align*}
$$
## Chain Rule
$$
\text{for a function } y=f(g(x)),\text{ where }g(x)=g,\\
\begin{align*}
\frac{\mathrm{d}y}{\mathrm{d}x}&=\lim_{\Delta x\to0}{\left[\frac{f(g(x+\Delta x))-f(g(x))}{\Delta x}\right]}\\
&=\lim_{\Delta x\to0}{\left[\frac{f(g(x+\Delta x))-f(g(x))}{\underbrace{g(x+\Delta x)-g(x)}_{=\Delta g}}\times\frac{g(x+\Delta x)-g(x)}{\Delta x}\right]}\\
&=\lim_{\Delta g\to0}{\left[\frac{f(g+\Delta g)-f(g)}{\Delta g}\right]}\times\lim_{\Delta x\to0}{\left[\frac{\Delta g}{\Delta x}\right]}\\
&=\frac{\mathrm{d}f(x)}{\mathrm{d}g(x)}\times\frac{\mathrm{d}g(x)}{\mathrm{d}x}
\end{align*}
$$
## Logarithm Rule
$$
\text{for a function } y=f(x)=b^x,\text{ where }f(x)=f,\\
\ln{f}=x\ln{b}\\
\therefore \frac{\mathrm{d}}{\mathrm{d}x}\ln{f}=\frac{\mathrm{d}}{\mathrm{d}x}x\ln{b}\\
\implies \frac{\mathrm{d}}{\mathrm{d}f}\ln{f}\times\frac{\mathrm{d}f}{\mathrm{d}x}=\ln{b}\\
\implies \frac{1}{f}\frac{\mathrm{d}f}{\mathrm{d}x}=\ln{b}\\
\therefore \frac{\mathrm{d}y}{\mathrm{d}x}=f(x)\ln{b}=b^x\ln{b}
$$
## Leibniz’ Theorem
The $n$th derivative of a product rule function $f(x)=u(x)\cdot v(x)$ can be written as follows:
$$
\frac{\mathrm{d}^{n}}{\mathrm{d}x^n}f(x)=\sum_{r=0}^{n}{\left[\binom{n}{r}\cdot\frac{\mathrm{d}^{n-r}}{\mathrm{d}x^{n-r}}u(x)\cdot\frac{\mathrm{d}^r}{\mathrm{d}x^r}v(x)\right]}
$$
## Inverse Function Rule
The derivative of a function is equal to the reciprocal of the derivative of the inverse function:
$$
f^{\prime}(x)=\frac{1}{{f^{-1}}^{\prime}(f(x))}
$$