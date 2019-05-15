The general idea of hypothesis testing involves:

1. Making an initial assumption.
2. Collecting evidence (data).
3. Based on the available evidence (data), deciding whether to reject or not reject the initial assumption.

Every hypothesis test — regardless of the population parameter involved — requires the above three steps.

### Is Normal Body Temperature Really 98.6 Degrees F?

Consider the population of many, many adults. A researcher hypothesized that the average adult body temperature is lower than the often-advertised 98.6 degrees F. 

That is, **the researcher wants an answer to the question: "Is the average adult body temperature 98.6 degrees? Or is it lower?"** 

To answer his research question, **the researcher starts by assuming that the average adult body temperature was 98.6 degrees F.**

Then, the researcher went out and tried to find evidence that refutes his initial assumption. In doing so, he selects a random sample of 130 adults. The average body temperature of the 130 sampled adults is 98.25 degrees.

Then, the researcher uses the data he collected to make a decision about his initial assumption. It is either *likely* or *unlikely* that the researcher would collect the evidence he did **given his initial assumption** that the average adult body temperature is 98.6 degrees:

- If it is *likely*, then the researcher **does not reject** his initial assumption that the average adult body temperature is 98.6 degrees. There is not enough evidence to do otherwise.
- If it is unlikely, then:
  - either the researcher's initial assumption is correct and he experienced a very unusual event;
  - or the researcher's initial assumption is incorrect.

In statistics, we generally don't make claims that require us to believe that a very unusual event happened. That is, in the practice of statistics, if the evidence (data) we collected is unlikely in light of the initial assumption, then we **reject** our initial assumption.

### Criminal Trial Analogy

One place where you can consistently see the general idea of hypothesis testing in action is in criminal trials held in the United States. Our criminal justice system assumes "the defendant is innocent until proven guilty." That is, our initial assumption is that the defendant is innocent.

In the practice of statistics, we make our initial assumption when we state our two competing hypotheses -- the null hypothesis (*H*0) and the alternative hypothesis (*H*A). 

Here, our hypotheses are:

- *H*0: Defendant is not guilty (innocent)
- *H*A: Defendant is guilty

In statistics, we always **assume the null hypothesis is true**. That is, the null hypothesis is always our initial assumption.

The prosecution team then collects evidence — such as finger prints, blood spots, hair samples, carpet fibers, shoe prints, ransom notes, and handwriting samples — with the hopes of finding "sufficient evidence" to make the assumption of innocence refutable.

In statistics, the **data** are the evidence.

The jury then makes a decision based on the available evidence:

- If the jury finds sufficient evidence — beyond a reasonable doubt — to make the assumption of innocence refutable, the jury **rejects the null hypothesis** and deems the defendant guilty. We behave as if the defendant is guilty.
- If there is insufficient evidence, then the jury **does not reject the null hypothesis**. We behave as if the defendant is innocent.

In statistics, we always make one of two decisions. We either "reject the null hypothesis" or we "fail to reject the null hypothesis.”

Note that, in statistics, we call the two types of errors by two different  names -- one is called a "Type I error," and the other is called  a "Type II error." Here are the formal definitions of the two types of errors:

- Type I Error

  The null hypothesis is rejected when it is true.

- Type II Error

  The null hypothesis is not rejected when it is false.

There is always a chance of making one of these errors. But, a good scientific study will minimize the chance of doing so.

### Making the decision

Recall that it is either *likely* or *unlikely* that we would observe the evidence we did given our initial assumption. If it is *likely*, we do not reject the null hypothesis. If it is *unlikely*, then we reject the null hypothesis in favor of the alternative hypothesis. Effectively, then, making the decision reduces to determining "likely" or "unlikely."

In statistics, there are two ways to determine whether the evidence is likely or unlikely given the initial assumption:

1. We could take the "**critical value approach**" (favored in many of the older textbooks).
2. Or, we could take the "***P*****-value approach**" (what is used most often in research, journal articles, and statistical software).

In the next two sections, we review the procedures behind each of these two approaches. To make our review concrete, let's imagine that *μ* is the average grade point average of all American students who major in mathematics. We first review the critical value approach for conducting each of the following three hypothesis tests about the population mean $\mu$,

| Type         | Null         | Alternative     |
| ------------ | ------------ | --------------- |
| Right-tailed | $H_0: \mu=3$ | $H_A : μ > 3$   |
| Left-tailed  | $H_0: \mu=3$ | $H_A : μ < 3$   |
| Two-tailed   | $H_0: \mu=3$ | $H_A : μ \neq3$ |
|              |              |                 |

### In Practice

- We would want to conduct the first hypothesis test if we were interested in concluding that the average grade point average of the group is more than 3.
- We would want to conduct the second hypothesis test if we were interested in concluding that the average grade point average of the group is less than 3.
- And, we would want to conduct the third hypothesis test if we were only interested in concluding that the average grade point average of the group differs from 3 (without caring whether it is more or less than 3).

Upon completing the review of the critical value approach, we review the *P*-value approach for conducting each of the above three hypothesis tests about the population mean μ. The procedures that we review here for both approaches easily extend to hypothesis tests about any other population parameter.

### Hypothesis Testing (Critical Value Approach)

The critical value approach involves determining "likely" or "unlikely" by determining whether or not the observed test statistic is more extreme than would be expected if the null hypothesis were true. That is, it entails comparing the observed test statistic to some cutoff value, called the "**critical value**." If the test statistic is more extreme than the critical value, then the null hypothesis is rejected in favor of the alternative hypothesis. If the test statistic is not as extreme as the critical value, then the null hypothesis is not rejected.

Specifically, the four steps involved in using the critical value approach to conducting any hypothesis test are:

1. Specify the null and alternative hypotheses.

2. Using the sample data and assuming the null hypothesis is true, calculate the value of the test statistic. To conduct the hypothesis test for the population mean $\mu$, we use t-statistics 
   $$
   t^{*}=\frac{\overline{x}-\mu}{s / \sqrt{n}}
   $$

which follows a ***t*-distribution** with ***n* - 1 degrees of freedom**.

3. Determine the critical value by finding the value of the known distribution of the test statistic such that the probability of making a Type I error — which is denoted α (greek letter "alpha") and is called the "**significance level of the test**" — is small (typically 0.01, 0.05, or 0.10).
4. Compare the test statistic to the critical value. If the test statistic is more extreme in the direction of the alternative than the critical value, reject the null hypothesis in favor of the alternative hypothesis. If the test statistic is less extreme than the critical value, do not reject the null hypothesis.

### Mean GPA

In our example concerning the mean grade point average, suppose we take a random sample of *n* = 15 students majoring in mathematics. Since *n* = 15, our test statistic *t** has *n* - 1 = 14 degrees of freedom. Also, suppose we set our significance level α at 0.05, so that we have only a 5% chance of making a Type I error.

#### Right-Tailed

The critical value for conducting the **right-tailed** test *H*0 : *μ* = 3 versus *H*A : *μ* > 3 is the *t*-value, denoted *t*α, *n* - 1, such that the probability to the *right* of it is α. It can be shown using either statistical software or a *t*-table that the critical value *t* 0.05,14 is 1.7613. That is, we would reject the null hypothesis *H*0 : *μ* = 3 in favor of the alternative hypothesis *H*A : *μ* > 3 if the test statistic *t** is greater than 1.7613. Visually, the rejection region is shaded red in the graph.

![right-tailed](/Users/laozhaotou/Desktop/right-tailed.png)

#### Left-Tailed

The critical value for conducting the **left-tailed** test *H*0 : *μ* = 3 versus *H*A : *μ* < 3 is the *t*-value, denoted *-t*(α, *n* - 1) , such that the probability to the *left* of it is α. It can be shown using either statistical software or a *t*-table that the critical value *-t*0.05,14 is -1.7613. That is, we would reject the null hypothesis *H*0 : *μ* = 3 in favor of the alternative hypothesis *H*A : *μ* < 3 if the test statistic *t** is less than -1.7613. Visually, the rejection region is shaded red in the graph.

![left-tailed](/Users/laozhaotou/Desktop/left-tailed.png)

#### Two-Tailed

There are two critical values for the **two-tailed** test *H*0 : *μ* = 3 versus *H*A : *μ* ≠ 3 — one for the left-tail denoted *-t*(α/2, *n* - 1) and one for the right-tail denoted *t*(α/2, *n* - 1). The value *-**t*(α/2, *n* - 1) is the *t*-value such that the probability to the *left* of it is α/2, and the value *t*(α/2, *n* - 1) is the *t*-value such that the probability to the *right* of it is α/2. It can be shown using either statistical software or a *t*-table that the critical value *-t*0.025,14 is -2.1448 and the critical value *t*0.025,14 is 2.1448. That is, we would reject the null hypothesis *H*0 : *μ* = 3 in favor of the alternative hypothesis *H*A : *μ* ≠ 3 if the test statistic t* is less than -2.1448 or greater than 2.1448. Visually, the rejection region is shaded red in the graph.

![distribution plot](/Users/laozhaotou/Desktop/distribution plot.png)

### Hypothesis Testing (P-Value Approach)

The *P*-value approach involves determining "likely" or "unlikely" by determining the probability — assuming the null hypothesis were true — of observing a more extreme test statistic in the direction of the alternative hypothesis than the one observed. If the *P*-value is small, say less than (or equal to) α, then it is "unlikely." And, if the *P*-value is large, say more than α, then it is "likely."

If the *P*-value is less than (or equal to) α, then the null hypothesis is rejected in favor of the alternative hypothesis. And, if the *P*-value is greater than α, then the null hypothesis is not rejected.

Specifically, the four steps involved in using the *P*-value approach to conducting any hypothesis test are:

1. Specify the null and alternative hypotheses.

2. Using the sample data and assuming the null hypothesis is true, calculate the value of the test statistic. Again, to conduct the hypothesis test for the population mean *μ*, we use the *t*-statistic 
   $$
   t^{*}=\frac{\overline{x}-\mu}{s / \sqrt{n}}
   $$
   which follows a *t*-distribution with *n* - 1 degrees of freedom.

3. Using the known distribution of the test statistic, calculate the ***P*****-value**: "If the null hypothesis is true, what is the probability that we'd observe a more extreme test statistic in the direction of the alternative hypothesis than we did?" (Note how this question is equivalent to the question answered in criminal trials: "If the defendant is innocent, what is the chance that we'd observe such extreme criminal evidence?")

4. Set the significance level, α, the probability of making a Type I error to be small — 0.01, 0.05, or 0.10. Compare the *P*-value to α. If the *P*-value is less than (or equal to) α, reject the null hypothesis in favor of the alternative hypothesis. If the *P*-value is greater than α, do not reject the null hypothesis.