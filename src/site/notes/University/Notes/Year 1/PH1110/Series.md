---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/series/","dg-note-properties":{}}
---

The sum of the series $a$ under inspection can be written in the following form:
$$
S=\sum^{\infty}_{n=N}{a_n}
$$
For a series beginning at term $N$ and ranging to $\infty$; where $a_n$ is term $n$ in the series.
# Tests for Convergence and Divergence
## Inspection
If each consecutive term is greater than the last ($a_{n+1}>a_n$), the series will diverge.
## Ratio Test
Define the ratio of consecutive terms $\rho_n$ as follows:
$$
\rho_n\equiv\left(\frac{a_{n+1}}{a_n}\right)
$$
Then, the limit of this as $n$ becomes arbitrarily large is $\rho$:
$$
\rho\equiv\lim_{n\to\infty}\rho_n
$$
$\rho$ describes the behaviour of the function:
$$
\text{If...}
\begin{cases}
\rho<1,&\text{convergent}\\
\rho=1,&\text{more tests required}\\
\rho>1,&\text{divergent}
\end{cases}
$$
## Integral Test
The sum $S$ can be expressed in integral form as follows:
$$
S=\sum^{\infty}_{n=N}{a_n}=\int_N^{\infty}{a_n}\ \mathrm{d}n
$$
Note that this integral cannot be used to evaluate the sum as the series does not represent a continuous function.
However, if the integral is finite, the series converges.
## Comparison Test
Find a similar series $m$ to compare to $a$. Then, if each term of $m$ is smaller than the corresponding term of $a$ ($\left|{a_n}\right|<\left|m_n\right|$) and $m$ converges, $a$ is also convergent.
## Alternating Series Test
For an alternating series, if each consecutive term is smaller than the last ($\left|a_{n+1}\right|<\left|a_n\right|$) and the terms tend to zero as $n$ becomes arbitrarily large $\lim_{n\to\infty}{a_n}=0$, then the series is convergent.