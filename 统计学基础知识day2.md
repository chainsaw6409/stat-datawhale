## Day 2 统计学基础知识

Recall that a random variable is said to have a normal distribution with parameters $\mu$ and $\sigma$ if it has a continuous distribution with density 
$$
f_{\mu, \sigma}(x)=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left(-\frac{(x-\mu)^{2}}{2 \sigma^{2}}\right) \quad \text { for }-\infty<x<\infty
$$
The normal distribution is denoted by $N(μ,σ2)​$. The parameter $σ​$ must be positive, otherwise the density would not be positive. The parameter $μ​$ can be any real value. 

The special case where$ μ = 0​$ and $σ = 1​$ is called the **standard normal**. The density function for this $N(0,1)​$ distribution is usually denoted by the special letter $φ​$,
$$
\phi(x)=\frac{1}{\sqrt{2 \pi}} e^{-x^{2} / 2} \quad \text { for }-\infty<x<\infty
$$
For this function to be a well defined desnity it must integrate to 1, that is,
$$
\int_{-\infty}^{\infty} e^{-x^{2} / 2} d x=\sqrt{2 \pi}
$$
X has a $N(μ,σ2)$ distribution if and only if $(*X* −μ)/σ$ has a standard normal distribution. That is, we can write $ X = μ+σ Z$ where *Z* has a standard normal distribution.

#### Example <1>

The$ N(μ,σ^2)​$ distribution has expected value $μ​$ and variance $σ^2​$.

The normal distribution also has an important stability property: if *X* and *Y* are independent, each with a normal distribution, then *X* + *Y* also has a normal distribution. This fact will follow from a more general fact about sums of independent random variables.

#### Example <2>

Suppose *X* has a continuous distribution with density *f* and *Y* has a continuous distribution with density *g*. If *X* and *Y* are independent then the random variable *Z* = *X* + *Y* has a continuous distribution with density
$$
h(z)=\int_{-\infty}^{\infty} g(z-x) f(x) d x \quad \text { for all real } z
$$
The integral expression for the density *h* in terms of *f* and *g* is called the **convolution formula**. The next Example shows the formula in action. It also serves as an advertisement for indicator functions. You won’t be needing this particular result to understand the general normal approximation. You could safely skip the details.

#### Example <3>

Example <7.3>: If *X* and *Y* are independent, each with the Uniform(0, 1) distribution, find the distribution of *X* + *Y* .

As promised, the convolution formula also establishes the key fact about sums of independent normals, as recorded in the next Example.

#### Example <4>

If *X*1 and *X*2 are independent random variables with *X*1 ∼*N*(μ1,σ12) and *X*2 ∼ *N*(μ2,σ2), then *X*1 + *X*2 ∼ *N*(μ1 +μ2,σ12 +σ2).

### The Central Limit Theorem

The normal approximation to the binomial is just one example of a general phenomenon corresponding to the mathematical result known as the **central limit theorem**. Roughly stated, the theorem asserts:

> *If X can be written as a sum of a large number of relatively small, independent random variables, then it has approximately a $ N(μ,σ^2)$ distribution, where $\mu=\mathbb{E} X$ and $σ 2 = var( X )$. Equivalently, the standardized variable $(X-\mu)/\sigma​$ has approximately a standard normal distribution.*

The normal distribution has many agreeable properties that make it easy to work with. Many statistical procedures have been developed under normality assumptions, with occasional offhand references to the central limit theorem to mollify anyone who doubts that all distributions are normal. Modern theory has been much concerned with possible harmful effects of unwarranted assumptions such as normality. The modern fix often substitutes huge amounts of computing for neat, closed-form, analytic expressions; but normality still lurks behind some of the modern data analytic tools.

The normal distribution has many agreeable properties that make it easy to work with. Many statistical procedures have been developed under normality assumptions, with occasional offhand references to the central limit theorem to mollify anyone who doubts that all distributions are normal. Modern theory has been much concerned with possible harmful effects of unwarranted assumptions such as normality. The modern fix often substitutes huge amounts of computing for neat, closed-form, analytic expressions; but normality still lurks behind some of the modern data analytic tools.

#### Things to remember

- If X can be written as a sum of a large number of relatively small, independent random variables, then it has approximately a $ N(μ,σ^2)​$ distribution, where $\mu=\mathbb{E} X​$ and $σ 2 = var( X )​$. Equivalently, the standardized variable $(X-\mu)/\sigma​$ has approximately a standard normal distribution.

#### Example. 

The $N(μ,σ^2)$ is a continuous distribution with density.
$$
f_{\mu, \sigma}(x)=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left(-\frac{(x-\mu)^{2}}{2 \sigma^{2}}\right) \quad \text { for }-\infty<x<\infty
$$
If *X* has this distribution then
$$
\mathbb{E} X=\int_{-\infty}^{\infty} x f_{\mu, \sigma}(x) d x
$$
Make the change of variable *y* = (*x* − μ)/σ to rewrite the integral as
$$
\frac{1}{\sigma \sqrt{2 \pi}} \int_{-\infty}^{\infty}(\mu+\sigma y) \exp \left(-y^{2} / 2\right) \sigma d y=\mu \int_{-\infty}^{\infty} \phi(y) d y+\sigma \int_{-\infty}^{\infty} y \phi(y) d y
$$
We know (from the fact that φ is a density function) that the coefficient of μ equals 1. Antisymmetry of $yφ(y)$ makes it integrate to 0. Thus $\mathbb{E}X = μ$.

Similarly,
$$
\operatorname{var}(X)=\mathbb{E}(X-\mu)^{2}=\int_{-\infty}^{\infty}(x-\mu)^{2} f_{\mu, \sigma}(x) d x=\sigma^{2} \int_{-\infty}^{\infty} y^{2} \phi(y) d y
$$
An integration-by-parts, using the fact that *d*φ(*y*)/*dy* = −*y*φ(*y*), simplifies the integral,
$$
\int_{-\infty}^{\infty}-y \frac{d \phi(y)}{d y} d y=[-y \phi(y)]_{-\infty}^{\infty}+\int_{-\infty}^{\infty} \phi(y) d y=1
$$
Thus, var(X) = $\sigma^2$.

we could also summarize the calcualtion by writing $X = \mu + \sigma Z$, with $*Z* ∼ *N* (0, 1),then note that 
$$
\begin{aligned} \mathbb{E} X &=\mu+\sigma \mathbb{E} Z=\mu+\sigma \times 0 \\ \operatorname{var}(X) &=\sigma^{2} \operatorname{var}(Z)=\sigma^{2} \times 1 \end{aligned}
$$
The changes of variables in the integrals were effectively reducing the problem to the case of a standard normal.

### Confidence Intervals

In statistical inference, one wishes to estimate population parameters using observed sample data.

A **confidence interval** gives an estimated range of values which is likely to include an unknown population parameter, the estimated range being calculated from a given set of sample data. (*Definition taken from Valerie J. Easton and John H. McColl's Statistics Glossary v1.1*)

The common notation for the parameter in question is $\theta$. Often, this parameter is the population mean $\mu$, which is estimated through the sample mean $\hat{x}$.

The ***level C*** of a confidence interval gives the probability that the interval produced by the method employed includes the true value of the parameter $\theta$.

### Example

Suppose a student measuring the boiling temperature of a certain liquid observes the readings (in degrees Celsius) 102.5, 101.7, 103.1, 100.9, 100.5, and 102.2 on 6 different samples of the liquid. He calculates the sample mean to be 101.82. If he knows that the standard deviation for this procedure is 1.2 degrees, what is the confidence interval for the population mean at a 95% confidence level?

In other words, the student wishes to estimate the true mean boiling temperature of the liquid using the results of his measurements. If the measurements follow a normal distribution, then the sample mean will have the distribution $\mathrm{N}\left(\mu, \frac{\sigma}{\sqrt{n}}\right)$. Since the sample size is 6, the standard deviation of the sample mean is equal to 1.2/sqrt(6) = 0.49.



> **The selection of a confidence level for an interval determines the probability that the confidence interval produced will contain the true parameter value.** 

Common choices for the confidence level C are 0.90, 0.95, and 0.99. These levels correspond to percentages of the area of the normal density curve. For example, a 95% confidence interval covers 95% of the normal curve -- the probability of observing a value outside of this area is less than 0.05. Because the normal curve is symmetric, half of the area is in the left tail of the curve, and the other half of the area is in the right tail of the curve. As shown in the diagram to the right, for a confidence interval with level C, the area in each tail of the curve is equal to (1-C)/2. For a 95% confidence interval, the area in each tail is equal to 0.05/2 = 0.025.

The value $z*$ representing the point on the standard normal density curve such that the probability of observing a value greater than$ z*$ is equal to *p* is known as the upper *p* critical value of the standard normal distribution. For example, if *p* = 0.025, the value $z*$ such that *P(Z > z\*)* = 0.025, or $P(Z < z*) = 0.975$, is equal to 1.96. For a confidence interval with level *C*, the value *p* is equal to (1-*C*)/2. A 95% confidence interval for the standard normal distribution, then, is the interval (-1.96, 1.96), since 95% of the area under the curve falls within this interval.

![confdiag](http://www.stat.yale.edu/Courses/1997-98/101/confdiag.gif)

