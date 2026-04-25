---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/integration/","dg-note-properties":{}}
---

# Definition from First Principles
The Reimann definition from first principles is:
$$
I=\int_a^b{f(x)}\,\mathrm{d}x=\lim_{n\to\infty}\sum_{i=1}^nf(x_i)\,\Delta x
$$
where $\Delta x=\dfrac{b-a}{n}$.
Which is equivalent to splitting a curve into intervals of width $\Delta x$ and evaluating the sum of the areas of these intervals as their widths tends towards zero.
As the interval width is defined as the integral range $[a,b]$ divided by the number of intervals $n$, we can express the limit of the widths as a limit of $n$.
For indefinite integrals, we must add a constant of integration $C$, which is an arbitrary constant.