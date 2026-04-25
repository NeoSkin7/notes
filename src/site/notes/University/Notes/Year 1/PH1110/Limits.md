---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/limits/","dg-note-properties":{}}
---

Limits allow for the approximation of complicated expressions and evaluation of indeterminate forms (e.g. $\frac{0}{0}$), allowing for expressions to be used in algebra. An example of their use is in the methods of calculus.
# Definition
The mathematical definition is: if $\lim\limits_{x\to a}{f(x)}=l$ then for a number $\varepsilon$, however small, it must be possible to find a number $\eta$ such that $\left|f(x)-l\right|<\varepsilon$ whenever $\left|x-a\right|<\eta$.
In other words, as $x$ becomes arbitrarily small compared to $a$, $f(x)$ becomes arbitrarily close to the limit $l$.
# Approaching Limits
Limits may be approached from above or below, and these may give different results:
$$
L=\lim_{x\to\frac{\pi}{2}}{\tan{x}}
\begin{cases}
\lim\limits_{x\uparrow \frac{\pi}{2}}{\tan{x}}=\lim\limits_{x\to\frac{\pi}{2}^+}{\tan{x}}=\lim\limits_{x\nearrow\frac{\pi}{2}}{\tan{x}}=\infty,&\text{from below/left}\\
\lim\limits_{x\downarrow\frac{\pi}{2}}{\tan{x}}=\lim\limits_{x\to\frac{\pi}{2}^-}{\tan{x}}=\lim\limits_{x\searrow\frac{\pi}{2}}{\tan{x}}=-\infty,&\text{from above/right}
\end{cases}
$$
# Simplifications
## Sums
$$
\lim_{x\to a}\left[f(x)+g(x)\right]=\lim_{x\to a}{f(x)}+\lim_{x\to a}{g(x)}
$$
## Products
$$
\lim_{x\to a}{f(x)g(x)}=\left[\lim_{x\to a}{f(x)}\right]\cdot\left[\lim_{x\to a}{g(x)}\right]
$$
## Exponents
$$
\lim_{x\to a}{\ln{y}}=b\iff \lim_{x\to a}{y}=e^b
$$
## Limits to Infinity and Zero
$$
\lim_{x\to \infty}{f(x)}=\lim_{y\to 0}{f\left(\frac{1}{y}\right)}
$$
where $y=\frac{1}{x}$.
# L’Hôpital’s Rule
When both $f(a)$ and $g(a)$ are equal to zero, their quotient cannot be evaluated in a limit. In this case, consider the Taylor expansion of both functions, to find:
$$
\lim_{x\to a}{\frac{f(x)}{g(x)}}=\lim_{x\to a}{\frac{f(a)+(x-a)f^{\prime}(a)+\frac{(x-a)^2}{2!}f^{\prime\prime}(a)+\cdots}{g(a)+(x-a)g^{\prime}(a)+\frac{(x-a)^2}{2!}g^{\prime\prime}(a)+\cdots}}=\lim_{x\to a}{\frac{f^{\prime}(a)+\frac{(x-a)}{2!}f^{\prime\prime}(a)+\cdots}{g^{\prime}(a)+\frac{(x-a)}{2!}g^{\prime\prime}(a)+\cdots}}=\lim_{x\to a}{\frac{f^{\prime}(x)}{g^{\prime}(x)}}
$$
If both $f^{\prime}(a)$ and $g^{\prime}(a)$ are also zero, the Taylor expansion can be revaluated:
$$
\lim_{x\to a}{\frac{f(x)}{g(x)}}=\lim_{x\to a}{\frac{f^{\prime\prime}(x)}{g^{\prime\prime}(x)}}
$$