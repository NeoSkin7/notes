---
{"dg-publish":true,"permalink":"/university/notes/year-1/ph-1110/probability-distributions/","dg-note-properties":{}}
---

# Probability Distribution Functions
Probabilities are often the result of interactions between variables, best expressed using functions. The probability of events occurring is given by the sum or integral over the functions:
$$
\mathbb{P}(a<x<b)=\int_a^b{f(x)}\ \mathrm{d}x,x\in[c,d]
$$
where $\int_c^d{f(x)}\ \mathrm{d}x=1$, the probability over the full function range is equal to one (normalisation condition).
## Mean
The distribution mean $\mu$ is given by:
$$
\mu=\int_c^d{xf(x)}\ \mathrm{d}x
$$
## Variance
An expression for the variance $\sigma^2$ is:
$$
\sigma^2=\int_c^d{(x-\mu)^2f(x)}\ \mathrm{d}x
$$
The standard deviation $\sigma$ is given by the square root of this value.
## Median
The median $m$ is found as the value at the midpoint of the range:
$$
\int_c^m{f(x)}\ \mathrm{d}x=\frac{1}{2}
$$
## Mode
The maximum value of the function gives the mode:
$$
f^{\prime}(M)=0
$$
# Standard Distributions
## Binomial
The binomial probability has the following form:
$$
\mathbb{P}_n(k)=\frac{n!}{k!(n-k)!}p^k(1-p)^{n-k}
$$
where the probability of $k$ events occurring from a set of $n$, each with probability $p$, is $\mathbb{P}_n(k)$.
This is a discrete distribution, so sums are used for calculations instead of integrals.
### Mean
The mean of the distribution is:
$$
\mu=\sum_{k=0}^n{k\mathbb{P}_n(k)}=np
$$
### Variance
The distribution variance is given by:
$$
\sigma^2=\langle k^2\rangle-\langle k\rangle^2=np(1-p)
$$
where $\langle k\rangle$ is the mean of $k$ events ($\mu$). The variance is literally the mean of the squares minus the square of the mean.
## Poisson
The form of the Poisson distribution is:
$$
\mathbb{P}(k)=e^{-\lambda}\frac{\lambda^k}{k!}
$$
where $\lambda$ is the mean rate of $k$ random events.
### Mean
The distribution mean is the same as the mean event rate.
### Variance
The variance is also equal to the mean event rate, meaning that the standard deviation is given by the square of the mean.
## Gaussian Distribution
A Gaussian or normal distribution follows the equation:
$$
p_G(x)=\frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{(x-\mu)^2}{2\sigma^2}}=\frac{1}{\sigma\sqrt{2\pi}}\exp{\left[-\frac{(x-\mu)^2}{2\sigma^2}\right]}
$$
with a probability given by:
$$
\mathbb{P}(x)=\int_a^b{p_G(x)}\ \mathrm{d}x
$$
where the probability of a large number of random events approaches the Gaussian probability according to the central limit theorem and the mean and standard deviation are distribution parameters.
### Central Limit Theorem
The central limit theorem states:
As the number of experiments becomes large, the random variable representing the average of the experiments tends to have a Gaussian distribution.
### Properties
The Gaussian distribution is:
- symmetric about the mean
- and continuous

with the median and mode falling in the same position as the mean.
The width of the distribution is determined by the standard deviation.
### Standard Distribution
The standard Gaussian distribution has a mean of zero and a standard deviation of one, giving:
$$
\varphi(z)=\frac{1}{\sqrt{2\pi}}e^{-\frac{z^2}{2}}=\frac{1}{\sqrt{2\pi}}\exp{\left[-\frac{z^2}{2}\right]}
$$
and, hence:
$$
p_G(x\mid \mu,\sigma)=\frac{1}{\sigma}\varphi\left(\frac{x-\mu}{\sigma}\right)
$$
as $z=\frac{x-\mu}{\sigma}$.
The cumulative distribution function $\Phi$ gives the probability of the standard random variable $z$ having a value greater than or equal to the input parameter $Z$:
$$
\Phi(Z)=\int_{-\infty}^Z{\varphi(z)}\ \mathrm{d}z
$$
### Cumulative Distribution
The cumulative distribution function of the full Gaussian distribution is:
$$
\mathbb{P}(X\le x)=\int_{-\infty}^{X}{p_G(x)}\ \mathrm{d}x=\frac{1}{\sigma\sqrt{2\pi}}\int_{-\infty}^{X}{e^{-\frac{(x-\mu)^2}{2\sigma^2}}}\ \mathrm{d}x=\frac{1}{\sigma\sqrt{2\pi}}\int_{-\infty}^{X}{\exp{\left[-\frac{(x-\mu)^2}{2\sigma^2}\right]}}\ \mathrm{d}x
$$
### Sigma Limits
The percentage of values that fall within multiples of sigma from the mean ($\mu\pm n\sigma$) of the Gaussian distribution is:
$$
\mathbb{P}(\mu-n\sigma\le x\le\mu+n\sigma)=
\begin{cases}
68.26\%,&\text{at }n=1\\
95.44\%,&\text{at }n=2\\
99.73\%,&\text{at }n=3\\
99.9937\%,&\text{at }n=4\\
99.999943\%,&\text{at }n=5\\
99.9999998\%,&\text{at }n=6
\end{cases}
$$