---
{"dg-publish":true,"permalink":"/year-1/ph-1110/algebra/de-moivre-s-theorem/","dg-note-properties":{}}
---

# Argument Rule
The argument of a product of two complex numbers is the sum of their arguments:
$$
\arg{z_1z_2}=\arg{z_1}+\arg{z_2}\\
\arg{\frac{z_1}{z_2}}=\arg{z_1}-\arg{z_2}
$$
# Modulus Rule
The modulus of a product of two complex numbers is the product of their moduli:
$$
\left|z_1z_2\right|=\left|z_1\right|\left|z_2\right|\\
\left|\frac{z_1}{z_2}\right|=\frac{\left|z_1\right|}{\left|z_2\right|}
$$
# De Moivre’s Theorem
Using both of the above rules, an expression can be derived using the polar form of a complex number for the multiplication of complex numbers:
$$
z_1z_2z_3\cdots z_n=r_1r_2r_3\cdots r_n\left[\cos{\left(\varphi_1+\varphi_2+\varphi_3+\cdots+\varphi_n\right)}+i\sin{\left(\varphi_1+\varphi_2+\varphi_3+\cdots+\varphi_n\right)}\right]
$$
When all of the complex numbers are equal, we can find the index of a complex number:
$$
z^n=r^n\left[\cos{n\varphi}+i\sin{n\varphi}\right]
$$
And, by extension:
$$
\frac{1}{z^n}=z^{-n}=r^{-n}\left[\cos{\left(-n\varphi\right)}+i\sin{\left(-n\varphi\right)}\right]=\frac{1}{r^n}\left[\cos{\left(-n\varphi\right)}+i\sin{\left(-n\varphi\right)}\right]
$$
In exponential form, De Moivre’s theorem can be written as follows:
$$
\left(e^{i\varphi}\right)^n=e^{in\varphi},n\in\mathbb{Z}
$$
Which is trivial, but useful.
# Derivations
## Trigonometric Identities
By comparing the square of a complex number using De Moivre’s theorem and through binomial expansion, two identities can be derived:
$$
\begin{cases}
z^2=r^2\left[\cos{2\varphi}+i\sin{2\varphi}\right]\\
z^2=r^2\left[\cos{\varphi}+i\sin{\varphi}\right]^2\\
\end{cases}
\text{ Let }r=1\ \therefore
\begin{cases}
z^2=\left[\cos{2\varphi}+i\sin{2\varphi}\right]\\
z^2=\left[\cos{\varphi}+i\sin{\varphi}\right]^2\\
\end{cases}\\
\implies\left[\cos{\varphi}+i\sin{\varphi}\right]^2=\left[\cos{2\varphi}+i\sin{2\varphi}\right]\\
\therefore\cos^2{\varphi}+2i\sin{\varphi}\cos{\varphi}-\sin^2{\varphi}=\cos{2\varphi}+i\sin{2\varphi}\\
\text{Comparing }\Re{(z)}\text{ and }\Im{(z)}:\\
\begin{cases}
\cos^2{\varphi}-\sin^2{\varphi}=\cos{2\varphi}\\
2\sin{\varphi}\cos{\varphi}=\sin{2\varphi}
\end{cases}
$$
## The $n$th Root of a Complex Number
By setting a complex number equal to a power of another, the root of the first can be found:
$$
\text{Consider }\omega^n=z:\\
\begin{cases}
z=r\left[\cos{\varphi}+i\sin{\varphi}\right]\\
\omega^n=\rho^n\left[\cos{n\vartheta}+i\sin{n\vartheta}\right]\\
\omega=\sqrt[n]{z}
\end{cases}\\
\implies r\left[\cos{\varphi}+i\sin{\varphi}\right]=\rho^n\left[\cos{n\vartheta}+i\sin{n\vartheta}\right]\\
\text{Which gives}:\\
\begin{cases}
\rho^n=r\\
n\vartheta=\varphi+2k\pi,k\in\mathbb{Z}
\end{cases}\\
\therefore
\begin{cases}
\rho=\sqrt[n]{r}\\
\vartheta=\dfrac{\varphi+2k\pi}{n},\{k\in\mathbb{Z}\mid0\le k\le(n-1)\}
\end{cases}
$$
Hence, the $n$th roots of a complex number are:
$$
\sqrt[n]{z}=\sqrt[n]{r}{\left[\cos{\frac{\varphi+2k\pi}{n}}+i\sin{\frac{\varphi+2k\pi}{n}}\right]}
$$
Or, alternatively:
$$
\sqrt[n]{z}=\sqrt[n]{r}e^{i\frac{\varphi+2k\pi}{n}}=\sqrt[n]{r}\exp{\left[i\frac{\varphi+2k\pi}{n}\right]}
$$
These roots are evenly distributed about the complex plane, forming equal angles with adjacent roots, and hence their sum is zero:
$$
\sqrt[n]{r}\sum_{k=0}^{n-1}{\left[\cos{\frac{\varphi+2k\pi}{n}}+i\sin{\frac{\varphi+2k\pi}{n}}\right]}=\sqrt[n]{r}\sum_{k=0}^{n-1}e^{i\frac{\varphi+2k\pi}{n}}=0
$$