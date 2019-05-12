# stat-datawhale

## Day 1 统计学基础知识

### Population mean & Sample mean

**In statistic, the arithmetic mean is one of the ideal measures of central tendency.** For a given set of observations, the arithmetic mean can be calculated by adding all the observations and dividing the value obtained by the number of observations. There are two types of mean, i.e. sample mean and population mean, which is often used in statistics and probability. The sample mean is mainly used to estimate the population mean when population mean is not known as they have the same expected value.

**Sample Mean** implies the mean of the sample derived from the whole population randomly. **Population Mean** is nothing but the average of the entire group. Take a glance at this article to know the differences between sample mean and population mean.



| BASIS FOR COMPARISON |                         SAMPLE MEAN                          |                       POPULATION MEAN                        |
| :------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|       Meaning        | Sample mean is the arithmetic mean of random sample values drawn from the population. | Population mean represents the actual mean of the whole population. |
|        Symbol        |                   x̄ (pronounced as x bar)                    |                      μ (Greek term mu)                       |
|     Calculation      |                             Easy                             |                          Difficult                           |
|       Accuracy       |                             Low                              |                             High                             |
|  Standard deviation  |    When calculated using sample mean, is denoted by (s).     |  When calculated using population mean, is denoted by (σ).   |

### Defination of Sample Mean

The sample mean is the mean **calculated from a group of random variables, drawn from the population.** It is regarded as an efficient and unbiased estimator of population mean which means that the most expected value for the sample statistic is the population statistic, irrespective of the sampling error. The sample mean is calculated as under:
$$
\overline{x}=\frac{1}{n} \sum_{i=1}^{n} a_{i}
$$
where, $n$ = Size of sample
$∑$ = Add up
$a_i$ = All the observations

### Definition of Population Mean

In, statistics, **population mean is defined as the average of the all the elements in the population.** It is a mean of group characteristic, where group refers to elements of the population like items, persons, etc. and the characteristic is the item of interest. As the population is very large and not known, the population mean is unknown constant. With the help of the following formula, population mean can be calculated,
$$
\mu=\frac{1}{N} \sum_{i=1}^{N} a_{i}
$$
where $N$ = Size of the population
$∑$ = Add up
$a_i$ = All the observations

### Key Differences Between Sample Mean and Population Mean

The significant differences between sample mean and population mean are explained in detail in the points given below:

1. The arithmetic mean of random sample values drawn from the population is called sample mean. The arithmetic mean of the entire population is called population mean.
2. The sample is represented by x̄ (pronounced as an x bar). On the other hand, population mean is labelled as μ (Greek term mu).
3. While the calculation of sample mean is easy, as the list of elements provided are only few which consumes very less time. As opposed to the population mean, where the calculation is difficult, as there are many elements in population which take a lot of time.
4. The accuracy of a population mean is comparatively higher than the sample mean. The accuracy of a sample mean can be enhanced by increasing the number of observations.
5. Elements of the population are represented by ‘N’ in population mean. On the contrary, ‘n’ in sample mean represents the size of the sample.
6. When the standard deviation is calculated using sample mean, it is denoted by letter ‘s’. Conversely, when population mean is used in the calculation of standard deviation, it is represented by sigma (σ).

### Conclusion

The method of calculation of both the means are same, i.e. sum of all observations divided by the number of observations, but there is a big difference between how they are represented. **While a sample mean is written as x̄ or sometimes M, population mean is labelled as μ. The sample mean is a random variable while population mean is an unknown constant.**

### Definition of Variance (population)

Variance measures how far a data set is spread out. The technical definition is *“The average of the squared differences from the mean,”* but all it really does is to give you a very **general idea of the spread of your data**. A value of zero means that there is no variability; All the numbers in the data set are the same.
$$
\sigma^{2}=\frac{\sum\left(x_{i}-\mu\right)^{2}}{N}
$$


### Sample Variance

**The sample variance, $s^2$, is used to calculate how varied a sample is.** A sample is a select number of items taken from a population. For example, if you are measuring American people’s weights, it wouldn’t be feasible (from either a time or a monetary standpoint) for you to measure the weights of every person in the population. The solution is to take a sample of the population, say 1000 people, and use that sample size to estimate the actual weights of the whole population. The variance helps you to figure out how spread out your weights are. 
$$
s^{2}=\frac{\sum\left(x_{i}-\overline{x}\right)^{2}}{n-1}
$$

#### Why n-1 for sample variance

![Screen Shot 2019-05-12 at 9.11.50 AM](/Users/laozhaotou/Desktop/Screen Shot 2019-05-12 at 9.11.50 AM.png)

## Population and sample standard deviation

Standard deviation measures the spread of a data distribution. It measures the typical distance between each data point and the mean.

The formula we use for standard deviation depends on whether the data is being considered a population of its own, or the data is a sample representing a larger population.

- If the data is being considered a population on its own, we divide by the number of data points, *N*.
- If the data is a sample from a larger population, we divide by one fewer than the number of data points in the sample, $n-1$.

**Population standard deviation**:
$$
\sigma=\sqrt{\frac{\sum\left(x_{i}-\mu\right)^{2}}{N}}
$$
**Sample standard deviation**:
$$
s_{x}=\sqrt{\frac{\sum\left(x_{i}-\overline{x}\right)^{2}}{n-1}}
$$


In statistics, the **standard deviation** (**SD**, also represented by the lower case Greek letter sigma **σ** or the Latin letter $s$) is a measure that is used to quantify the amount of variation or dispersion of a set of data values.low standard deviation indicates that the data points tend to be close to the mean (also called the expected value) of the set, while a high standard deviation indicates that the data points are spread out over a wider range of values.
$$

$$
where ${\displaystyle \textstyle \{x_{1},\,x_{2},\,\ldots ,\,x_{N}\}}$are the observed values of the sample items, $\bar{x}$ is the mean value of these observations, and $N$ is the number of observations in the sample.

### Random Varibles

In probability and statistics, a **random variable**, **random quantity**, **aleatory variable**, or **stochastic variable** is described informally as a variable whose values depend on outcomes of a [random](https://en.wikipedia.org/wiki/Randomness) phenomenon. 

A **random variable**, usually written *X*, is a variable whose possible values are numerical outcomes of a random phenomenon. There are two types of random variables, **discrete** and **continuous**.

The formal mathematical treatment of random variables is a topic in [probability theory](https://en.wikipedia.org/wiki/Probability_theory). In that context, a random variable is understood as a [measurable function](https://en.wikipedia.org/wiki/Measurable_function) defined on a [sample space](https://en.wikipedia.org/wiki/Sample_space) whose outcomes are typically real numbers.

A random variable's possible values might represent the possible outcomes of a yet-to-be-performed experiment, or the possible outcomes of a past experiment whose already-existing value is uncertain.

## Discrete Random Variables

A *discrete random variable* is one which may take on only a countable number of distinct values such as 0,1,2,3,4,........ Discrete random variables are usually (but not necessarily) counts. If a random variable can take only a finite number of distinct values, then it must be discrete. Examples of discrete random variables include the number of children in a family, the Friday night attendance at a cinema, the number of patients in a doctor's surgery, the number of defective light bulbs in a box of ten.

The **probability distribution** of a discrete random variable is a list of probabilities associated with each of its possible values. It is also sometimes called the probability function or the probability mass function.



#### For example

Suppose a variable X can take the values 1, 2, 3, or 4. 

The probabilities associated with each outcome are described by the following table:

```
	Outcome 	1	2	3	4
	Probability	0.1	0.3	0.4	0.2
```

The probability that X is equal to 2 or 3 is the sum of the two probabilities: 

P(X = 2 or X = 3) = P(X = 2) + P(X = 3) = 0.3 + 0.4 = 0.7. 

Similarly, the probability that X is greater than 1 is equal to 

1 - P(X = 1) = 1 - 0.1 = 0.9, by the complement rule.

This distribution may also be described by the **probability histogram** shown down the bottom:

![pdf](http://www.stat.yale.edu/Courses/1997-98/101/pdf.gif)

All random variables (discrete and continuous) have a **cumulative distribution function**. It is a function giving the probability that the random variable *X* is less than or equal to *x*, for every value *x*. For a discrete random variable, the cumulative distribution function is found by summing up the probabilities.

#### For example

The cumulative distribution function for the above probability distribution is calculated as follows: 

The probability that X is less than or equal to 1 is 0.1, 

the probability that X is less than or equal to 2 is 0.1+0.3 = 0.4, 

the probability that X is less than or equal to 3 is 0.1+0.3+0.4 = 0.8, and 

the probability that X is less than or equal to 4 is 0.1+0.3+0.4+0.2 = 1.

The probability histogram for the cumulative distribution of this random variable is shown down the bottom
![pdf](http://www.stat.yale.edu/Courses/1997-98/101/pdf.gif)

## Continuous Random Variables

A *continuous random variable* is one which takes an infinite number of possible values. Continuous random variables are usually measurements. Examples include height, weight, the amount of sugar in an orange, the time required to run a mile.

A continuous random variable is not defined at specific values. Instead, it is defined over an *interval* of values, and is represented by the ***area under a curve*** (in advanced mathematics, this is known as an *integral*). The probability of observing any single value is equal to 0, since the number of values which may be assumed by the random variable is infinite.

Suppose a random variable *X* may take all values over an interval of real numbers. Then the probability that *X* is in the set of outcomes *A, P(A)*, is defined to be the area above *A* and under a curve. The curve, which represents a function *p(x)*, must satisfy the following:

***1:** The curve has no negative values (p(x) > 0 for all x)*

***2:** The total area under the curve is equal to 1.*

A curve meeting these requirements is known as a ***density curve***.

#### The Uniform Distribution

A random number generator acting over an interval of numbers (a,b) has a continuous distribution. Since any interval of numbers of equal width has an equal probability of being observed, the curve describing the distribution is a rectangle, with constant height across the interval and 0 height elsewhere. Since the area under the curve must be equal to 1, the length of the interval determines the height of the curve.

The following graphs plot the density curves for random number generators over the intervals (4,5) (top left), (2,6) (top right), (5,5.5) (lower left), and (3,5) (lower right). The distributions corresponding to these curves are known as ***uniform distributions***.



![unif](http://www.stat.yale.edu/Courses/1997-98/101/unif.gif)

### The Normal Distribution

**Definition.** The continuous random variable *X* follows a **normal distribution** if its probability density function is defined as:

A normal distribution has a bell-shaped density curve described by its mean $\mu$ and standard deviation $\sigma$. The density curve is symmetrical, centered about its mean, with its spread determined by its standard deviation. The height of a normal density curve at a given point x is given by
$$
\frac{1}{\sigma \sqrt{2 \pi}} e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^{2}}
$$
The **Standard Normal** curve, shown here, has mean 0 and standard deviation 1. If a dataset follows a normal distribution, then about 68% of the observations will fall within $\sigma$ of the mean $\mu$ , which in this case is with the interval (-1,1). About 95% of the observations will fall within 2 standard deviations of the mean, which is the interval (-2,2) for the standard normal, and about 99.7% of the observations will fall within 3 standard deviations of the mean, which corresponds to the interval (-3,3) in this case. Although it may appear as if a normal distribution does not include any values beyond a certain interval, the density is actually positive for all values, $ ({-\infty},{+\infty})  $

Data from any normal distribution may be transformed into data following the standard normal distribution by subtracting the mean $\mu $ and dividing by the standard deviation $\sigma $.

### Characteristics of a Normal Curve

It is the following known characteristics of the normal curve that directed me in drawing the curve as I did so above.

1) All normal curves are **bell-shaped** with points of inflection at *μ* ± *σ*.

2) All normal curves are **symmetric about the mean** ***μ***.

All normal curves are symmetric about the mean *μ*, because *f*(*μ*+*x*) = *f*(*μ*−*x*) for all *x*. That is:
$$
f(\mu+x)=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left\{-\frac{1}{2}\left(\frac{x+\mu-\mu}{\sigma}\right)^{2}\right\}=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left\{-\frac{1}{2}\left(\frac{x}{\sigma}\right)^{2}\right\}
$$
Equals:
$$
f(\mu-x)=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left\{-\frac{1}{2}\left(\frac{\mu-x-\mu}{\sigma}\right)^{2}\right\}=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left\{-\frac{1}{2}\left(\frac{-x}{\sigma}\right)^{2}\right\}=\frac{1}{\sigma \sqrt{2 \pi}} \exp \left\{-\frac{1}{2}\left(\frac{x}{\sigma}\right)^{2}\right\}
$$
Therefore, by the definition of symmetry, the normal curve is symmetric about the mean *μ.*

3) The area under an entire normal curve is 1.

4) All normal curves are positive for all *x*. That is, *f*(*x*) > 0 for all *x*.

5) The limit of *f(x*) as *x* goes to infinity is 0, and the limit of *f(x*) as *x* goes to negative infinity is 0. That is:
$$
\lim _{x \rightarrow \infty} f(x)=0 \text { and } \lim _{x \rightarrow-\infty} f(x)=0
$$
6) The height of any normal curve is maximized at *x* = µ.

Using what we know from our calculus studies, to find the point at which the maximum occurs, we must differentiate *f*(*x*) with respect to *x* and solve for *x* to find the maximum. Because our *f*(*x*) contains the natural exponential function, however, it is easier to take the derivative of the natural log of *f*(*x*) with respect to *x* and solve for *x* to find the maximum. [The maximum of *f*(*x*) is the same as the maximum of the natural log of *f*(*x*), because *loge*(*x*) is an increasing function of *x*. That is, *x*1 < *x*2 implies that *loge*(*x*1) < *loge*(*x*2). Therefore, *f*(*x*1) < *f*(*x*2) implies *loge*(*f*(*x*1) < *loge*(*f*(*x*2)).] That said, taking the natural log of *f*(*x*), we get:
$$
\log _{e}(f(x))=\log \left(\frac{1}{\sigma \sqrt{2 \pi}}\right)-\frac{1}{2 \sigma^{2}}(x-\mu)^{2}
$$
Taking the derivative of $ log_e(f(x)) $with respect to *x*, we get:
$$
\frac{d \log f(x)}{d x}=-\frac{1}{2 \sigma^{2}} \cdot 2(x-\mu)
$$
Now, setting the derivative of $ log_e(f(x)) $ to 0:
$$
\frac{d \log f(x)}{d x}=-\frac{1}{2 \sigma^{2}} \cdot 2(x-\mu) \overline{s E T}^{\overline{\equiv}} 0
$$


and solving for *x*, we get that *x* = *μ*. Taking the second derivative of *loge*(*f*(*x*)) with respect to *x*, we get:
$$
\frac{d^{2} \log f(x)}{d x^{2}}=-\frac{1}{\sigma^{2}}
$$
Because the second derivative of $ log_e(f(x)) $ is negative (for all *x*, in fact),  the point *x* = *μ* is deemed a local maximum.

7) The shape of any normal curve depends on its mean *μ* and standard deviation *σ*.

Given that the curve *f*(*x*) depends only on *x* and the two parameters *μ* and *σ*, the claimed characteristic is quite obvious. An example is perhaps more interesting than the proof.  Here is a picture of three superimposed normal curves —one of a *N*(0, 9) curve, one of a *N*(0, 16) curve, and one of a *N*(1, 9) curve:

![curve](/Users/laozhaotou/Desktop/curve.gif)



### Probability Density Function (PDF)

A continuous random variable takes on an uncountably infinite number of possible values. For a discrete random variable *X* that takes on a finite or countably infinite number of possible values, we determined $P(X = x) $for all of the possible values of *X*, and called it the probability mass function ("p.m.f."). For continuous random variables, as we shall soon see, the probability that *X* takes on any particular value *x* is 0. That is, finding *P*(*X* = *x*) for a continuous random variable *X* is not going to work. Instead, we'll need to find the probability that *X* falls in some interval (*a*, *b*), that is, we'll need to find *P*(*a* < *X* < *b*). We'll do that using a probability density function ("p.d.f."). 

Definition.

 The probability density function (“p.d.f”) of a continuous random variable $X$ with support$ S$ is an integrable function f(x) satisfying the following:

(1) *f*(*x*) is positive everywhere in the support *S*, that is, *f*(*x*) > 0, for all *x* in *S*

(2) The area under the curve *f*(*x*) in the support *S* is 1, that is:

$∫_Sf(x)dx=1$

(3) If *f*(*x*) is the p.d.f. of *x*, then the probability that *x* belongs to *A*, where *A* is some interval, is given by the integral of *f*(*x*) over that interval, that is:

$P(X∈A)=∫_Af(x)dx$

### Cumulative Distribution Functions

cumulative distribution function is defined for discrete random variables as:
$$
F(x)=P(X \leq x)=\sum_{t \leq x} f(t)
$$
*F*(*x*) accumulates all of the probability less than or equal to *x*. The cumulative distribution function for continuous random variables is just a straightforward extension of that of the discrete case. All we need to do is replace the summation with an integral.

**Definition.** The **cumulative distribution function** ("**c.d.f.***"*) of a continuous random variable *X* is defined as:
$$
F(x)=\int_{-\infty}^{x} f(t) d t
$$
for −∞ < *x* < ∞.

for discrete random variables, that *F*(*x*) is, in general, a non-decreasing *step* function. For continuous random variables, *F*(*x*) is a non-decreasing *continuous* function. 

To determine the distribution of a discrete random variable we can either provide its PMF or CDF. For continuous random variables, the CDF is well-defined so we can provide the CDF. However, the PMF does not work for continuous random variables, because for a continuous random variable $P(X=x)=0$  for all $x∈ℝ$. Instead, we can usually define the **probability density function (PDF)**. The PDF is the **density** of probability rather than the probability mass. The concept is very similar to mass density in physics: its unit is probability per unit length. To get a feeling for PDF, consider a continuous random variable XX and define the function $fx(x)$ as follows (wherever the limit exists):
$$
f_{X}(x)=\lim _{\Delta \rightarrow 0^{+}} \frac{P(x<X \leq x+\Delta)}{\Delta}
$$
The function $fX(x)$ gives us the probability density at point xx. It is the limit of the probability of the interval $(x,x+Δ]$divided by the length of the interval as the length of the interval goes to 0. Remember that
$$
P(x<X \leq x+\Delta)=F_{X}(x+\Delta)-F_{X}(x)
$$
So, 
$$
f_{X}(x)=\lim _{\Delta \rightarrow 0} \frac{F_{X}(x+\Delta)-F_{X}(x)}{\Delta}=\frac{d F_{X}(x)}{d x}=F_{X}^{\prime}(x)
$$
if $FX(x)$ is differentiable at x.

### The Binomial Distribution

In many cases, it is appropriate to summarize a group of independent observations by the number of observations in the group that represent one of two outcomes. For example, the proportion of individuals in a random sample who support one of two political candidates fits this description. In this case, the statistic $\hat{p}$ is the count X of voters who support the candidate divided by the total number of individuals in the group $n$. This provides an estimate of the parameter $p$, the proportion of individuals who support the candidate in the entire population. The ***binomial distribution*** describes the behavior of a count variable *X* if the following conditions apply:

***1:** The number of observations n is fixed.*

***2:** Each observation is independent.*

***3:** Each observation represents one of two outcomes ("success" or "failure").*

***4:** The probability of "success" p is the same for each outcome.*

If these conditions are met, then X has a binomial distribution with parameters $n$ and $p$, abbreviated $B(n,p)$.

**The probability that a random variable X with binomial distribution B(n,p) is equal to the value k, where k = 0, 1,....,n , is given by** 
$$
P(X=k)=\left( \begin{array}{l}{n} \\ {k}\end{array}\right) p^{k}(1-p)^{n-k}
$$
where, 
$$
\left( \begin{array}{l}{n} \\ {k}\end{array}\right)=\frac{n !}{k !(n-k) !}
$$
The latter expression is known as the ***binomial coefficient***, stated as "*n choose k*," or the number of possible ways to choose *k* "successes" from *n* observations. For example, the number of ways to achieve 2 heads in a set of four tosses is "4 choose 2", or 4!/2!2! = 6. The possibilities are {HHTT, HTHT, HTTH, TTHH, THHT, THTH}, where "H" represents a head and "T" represents a tail. The binomial coefficient multiplies the probability of *one* of these possibilities (which is (1/2)²(1/2)² = 1/16 for a fair coin) by the number of ways the outcome may be achieved, for a total probability of 6/16.

### Mean and variance of the Binomial Distribution

The binomial distribution for a random variable *X* with parameters *n* and *p* represents the sum of *n* independent variables *Z* which may assume the values 0 or 1. If the probability that each *Z* variable assumes the value 1 is equal to *p*, then the [mean](http://www.stat.yale.edu/Courses/1997-98/101/rvmnvar.htm#rvmean) of each variable is equal to *1\*p + 0\*(1-p) = p*, and the [variance](http://www.stat.yale.edu/Courses/1997-98/101/rvmnvar.htm#rvvar) is equal to *p(1-p).* By the addition properties for independent random variables, the mean and variance of the binomial distribution are equal to the sum of the means and variances of the *n* independent *Z* variables, so,
$$
\begin{array}{l}{\mu_{X}=n p} \\ {\sigma_{X}^{2}=n p(1-p)}\end{array}
$$
These definitions are intuitively logical. Imagine, for example, 8 flips of a coin. If the coin is fair, then *p* = 0.5. One would expect the mean number of heads to be half the flips, or *np* = 8*0.5 = 4. The variance is equal to *np(1-p)* = 8*0.5*0.5 = 2.

### Expectations

If you have a collection of numbers a1,a2,...,aNa1,a2,...,aN, their average is a single number that describes the whole collection. Now, consider a random variable XX. We would like to define its average, or as it is called in probability, its **expected value** or **mean**. The expected value is defined as the weighted average of the values in the range.

*Expected value* (= mean=average):
**Definition** 
Let XX be a discrete random variable with range $R_X={x1,x2,x3,…}$(finite or countably infinite). The *expected* value of X, denoted by EX is defined as
$$
E X=\sum_{x k \in R X} x_{k} \mathrm{P}\left(X=x_{k}\right)=\sum_{x \in R X} x_{k} P_{X}\left(x_{k}\right)
$$
To understand the concept behind EX, consider a discrete random variable with range $RX={x1,x2,x3,…}$. This random variable is a result of random experiment. Suppose that we repeat this experiment a very large number of times NN, and that the trials are independent. Let $N_1$ be the number of times we observe x1x1, $N_2$ be the number of times we observe x2, ...., Nk be the number of times we observe xkxk, and so on. Since $P(X=x_k)=P_X(xk)$, we expect that
$$
\begin{aligned} P_{X}\left(x_{1}\right) & \approx \frac{N_{1}}{N} \\ P_{X}\left(x_{2}\right) & \approx \frac{N_{2}}{N} \\ & \cdot \\ P_{X}\left(x_{k}\right) & \approx \frac{N_{k}}{N} \\ & . \end{aligned}
$$
In other words, we have $N_k≈NP_X(xk)$. Now, if we take the average of the observed values of X, we obtain

![Screen Shot 2019-05-12 at 12.14.23 PM](/Users/laozhaotou/Desktop/Screen Shot 2019-05-12 at 12.14.23 PM.png)



### The Poisson Probability Distribution

The Poisson Distribution was developed by the French mathematician Simeon Denis Poisson in 1837.

**The Poisson random variable** satisfies the following conditions:

1. The number of successes in two disjoint time intervals is independent.
2. The probability of a success during a small time interval is proportional to the entire length of the time interval.

Apart from disjoint time intervals, the Poisson random variable also applies to **disjoint regions of space**.

Applications

- the number of deaths by horse kicking in the Prussian army (first application)
- birth defects and genetic mutations
- rare diseases (like Leukemia, but not AIDS because it is infectious and so not independent) - especially in legal cases
- car accidents
- traffic flow and ideal gap distance
- number of typing errors on a page
- hairs found in McDonald's hamburgers
- spread of an endangered animal in Africa
- failure of a machine in one month

The **probability distribution of a Poisson random variable** *X* representing the number of successes occurring in a given time interval or a specified region of space is given by the formula:
$$
P(X)=\frac{e^{-\mu} \mu^{x}}{x !}
$$
where, 

$x=0,1,2,3…$

$e=2.71828$

$\mu=$mean number of successes in the given time interval or region of space$

If $μ$ is the average number of successes occurring in a given time interval or region in the Poisson distribution, then the mean and the variance of the Poisson distribution are both equal to $μ$.

$E(X)= \mu$

and

$V(X)=\sigma^2 = \mu$

Note: in a Poisson distribution, only one parameter, $\mu$ is needed to determine the probability of an event. 
