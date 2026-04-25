---
{"dg-publish":true,"permalink":"/year-1/ph-1110/algebra/complex-logarithms/","dg-note-properties":{}}
---

# Principle Argument
The principle argument of a complex number $\operatorname{Arg}{z}$ is the first value of the argument function - the value closest in magnitude to zero:
$$
\text{for a complex number }z=a+bi,\\
\operatorname{Arg}{z}=\tan{\frac{b}{a}}\\
\arg{z}=\operatorname{Arg}{z}+2k\pi,k\in\mathbb{Z}
$$
# Complex Natural Logarithms
By setting a complex number equal to an exponential of a complex number, we can derive an expression for the natural logarithm of a complex number:
$$
\text{Consider }z=e^\omega:\\
\omega=x+iy=\ln{\left|z\right|}+i\arg{z}\\
\implies\ln{z}=\ln{\left|z\right|}+i\arg{z}=\ln{\left|z\right|}+i(\operatorname{Arg}{z}+2k\pi)
$$
## Principle Logarithm
As there are multiple possible values for the logarithm of a complex number (from the argument definition), we define a principle logarithm in a similar was to the principle argument:
$$
\operatorname{Ln}{z}=\operatorname{Ln}{\left|z\right|}+i\operatorname{Arg}{z}
$$
# The Logarithm of a Negative Number
Previously, the logarithm of a negative number was undefined, but, by treating a negative number in the same way as a complex number, we can define the principle natural logarithm of a negative number:
$$
\operatorname{Ln}{\left(-n\right)}=\operatorname{Ln}{n}+i\pi
$$
As the principle argument of a negative number is $i\pi$.
This definition can be extended for all natural logarithms as:
$$
\ln{\left(-n\right)}=\ln{n}+i\left(\pi+2k\pi\right),k\in\mathbb{Z}
$$