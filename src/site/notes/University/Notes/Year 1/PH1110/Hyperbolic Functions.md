---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/hyperbolic-functions/","dg-note-properties":{}}
---

The hyperbolic functions are defined as follows:
$$
\begin{align*}
\sinh{x}&=\frac{e^x-e^{-x}}{2}\\
\cosh{x}&=\frac{e^x+e^{-x}}{2}\\
\tanh{x}&=\frac{\sinh{x}}{\cosh{x}}=\frac{e^x-e^{-x}}{e^x+e^{-x}}=\frac{e^{2x}-1}{e^{2x}+1}
\end{align*}
$$
With the reciprocal functions defined in the same way as for the trigonometric functions.
# Parity
The parity of the hyperbolic functions is the same as for the trigonometric functions, whereby $\sinh{x}$ is odd and $\cosh{x}$ is even.
# Relations to Trigonometric Functions
These functions can be related to their trigonometric counterparts:
<!-- Column 1 -->
$$
\begin{cases}
\sinh{x}=-i\sin{ix}\\
\cosh{x}=\cos{ix}\\
\tanh{x}=-i\tan{ix}
\end{cases}
$$

<!-- Column 2 -->
$$
\begin{cases}
\sin{x}=-i\sinh{ix}\\
\cos{x}=\cosh{ix}\\
\tan{x}=-i\tanh{ix}
\end{cases}
$$

<!-- Column 3 -->
$$
\begin{cases}
\sin{ix}=i\sinh{x}\\
\cos{ix}=\cosh{x}\\
\tan{ix}=i\tanh{x}
\end{cases}
$$
# Identities
The following identities can be derived for hyperbolic functions from their definitions in terms of trigonometric functions:
## Pythagorean Identities
$$
\begin{align*}
\sin^2{x}+\cos^2{x}=1&\implies\cosh^2{x}-\sinh^2{x}=1\\
\sec^2{x}=1-\tan^2{x}&\implies\operatorname{sech}^2{x}=1-\tanh^2{x}\\
\csc^2{x}=1+\cot^2{x}&\implies\operatorname{csch}^2{x}=\coth^2{x}-1
\end{align*}
$$
## Euler’s Formula
$$
\begin{align*}
\cos{x}+i\sin{x}=e^{ix}&\implies\cosh{x}+\sinh{x}=e^x\\
\cos{x}-i\sin{x}=e^{-ix}&\implies\cosh{x}-\sinh{x}=e^{-x}
\end{align*}
$$
## Angle Addition Formulae
$$
\begin{align*}
\sin{(\alpha+\beta)}=\sin{\alpha}\cos{\beta}+\sin{\beta}\cos{\alpha}&\implies\\&\sinh{(\alpha+\beta)}=\sinh{\alpha}\cosh{\beta}+\sinh{\beta}\cosh{\alpha}\\&\sinh{2x}=2\sinh{x}\cosh{x}\\
\cos{(\alpha+\beta)}=\cos{\alpha}\cos{\beta}-\sin{\alpha}\sin{\beta}&\implies\\&\cosh{(\alpha+\beta)=\cosh{\alpha}\cosh{\beta}+\sinh{\alpha}\sinh{\beta}}\\&\cosh{2x}=\cosh^2{x}+\sinh^2{x}
\end{align*}
$$
# Inverse Functions
The inverse hyperbolic functions are defined as follows:
$$
\operatorname{arsinh}{x}=\ln{\left(\sqrt{1+x^2}+x\right)}\\
\operatorname{arcosh}{x}=\ln{\left(\sqrt{x^2-1}+x\right)}\\
\operatorname{artanh}{x}=\ln{\sqrt{\frac{1+x}{1-x}}}
$$
Note the use of the $\operatorname{ar-}$ prefix instead of $\operatorname{arc-}$. This is used as the inverse hyperbolic functions find an area instead of an arc length.
These definitions can be derived using Euler’s formula, for $\operatorname{arsinh}{x}$, this derivation is:
$$
y=\operatorname{arsinh}{x}\implies x=\sinh{y}\\
e^y=\cosh{y}+\sinh{y}\\
\implies e^y=\sqrt{1+\sinh^2{y}}+\sinh{y}\\
\therefore e^y=\sqrt{1+x^2}+x\\
\implies y=\ln{\left(\sqrt{1+x^2}+x\right)}=\operatorname{arsinh}{x}
$$
# Derivatives
Some common derivatives of the hyperbolic functions are given below:
$$
\begin{align*}
\frac{\mathrm{d}}{\mathrm{d}x}\sinh{x}&=\cosh{x}\\
\frac{\mathrm{d}}{\mathrm{d}x}\cosh{x}&=\sinh{x}\\
\frac{\mathrm{d}}{\mathrm{d}x}\tanh{x}&=\operatorname{sech}^2{x}\\
\frac{\mathrm{d}}{\mathrm{d}x}\operatorname{sech}{x}&=\operatorname{sech}{x}\tanh{x}\\
\frac{\mathrm{d}}{\mathrm{d}x}\operatorname{csch}{x}&=\operatorname{csch}{x}\coth{x}\\
\frac{\mathrm{d}}{\mathrm{d}x}\coth{x}&=-\operatorname{csch}^2{x}
\end{align*}
$$
# Integration by Substitution
Hyperbolic functions can be used as a substitution in integration, for example:
$$
I=\int{\frac{1}{\sqrt{x^2+a^2}}}\ \mathrm{d}x\\
\text{Let }x=a\sinh{u}\implies \mathrm{d}x=a\cosh{u}\ \mathrm{d}u\\
\therefore I=\int{\frac{a\cosh{u}}{\sqrt{a^2\left(1+\sinh^2{u}\right)}}}\ \mathrm{d}u=\int{\frac{a\cosh{u}}{\sqrt{a^2\cosh^2{u}}}}\ \mathrm{d}u\\
\implies I=\int{1}\ \mathrm{d}u=u+C=\operatorname{arsinh}{\left(\frac{x}{a}\right)}+C
$$