---
{"dg-publish":true,"permalink":"/year-1/ph-1110/algebra/euler-s-formula/","dg-note-properties":{}}
---

Euler’s formula relates the exponential form of a unit complex number to its polar form:
$$
\hat{z}=e^{i\varphi}=\cos{\varphi}+i\sin{\varphi}=\frac{1}{r}\left(a+bi\right)
$$
This was derived in [Taylor and Maclaurin Expansions](/2ca052c198088090a3d6f399bc6f7f89).
And, hence:
$$
z=a+bi=r\left[\cos{\varphi}+i\sin{\varphi}\right]=re^{i\varphi}
$$
# Trigonometric Definitions
Using Euler’s formula, it is possible to derive definitions of the sine and cosine functions in terms of complex exponentials:
$$
e^{i\varphi}=\cos{\varphi}+i\sin{\varphi}\text{ and }e^{-i\varphi}=\cos{\varphi}-i\sin{\varphi}\\
\therefore\begin{cases}
e^{i\varphi}+e^{-i\varphi}=2\cos{\varphi}\\
e^{i\varphi}-e^{-i\varphi}=2i\sin{\varphi}
\end{cases}\\
\implies\begin{cases}
\cos{\varphi}=\dfrac{e^{i\varphi}+e^{-i\varphi}}{2}\\
\sin{\varphi}=\dfrac{e^{i\varphi}-e^{-i\varphi}}{2i}
\end{cases}
$$