# 7 Most Asked Questions on Central Limit Theorem
(Understanding the Importance of the Central Limit Theorem)
## 1. What is the Central Limit Theorem?
Given a sufficiently large sample size, the sampling distribution of the sample mean will approximate a normal distribution regardless of the data distribution in the population.
## 2. What is Sampling Distribution?
'Sampling distribution' describes the distribution of a sample statistic (e.g., the sample mean) over many samples from the same population (i.e., repeated sampling).
## 3. What are the conditions of the Central Limit Theorem?
1.	The sample size is sufficiently large.
2.	The samples are independent and identically distributed (IID) random variables.
3.	The population distribution has finite variance.
## 4. Does Central Limit Theorem work if the population distribution is NOT normal? Yes!
The sampling distribution of the sample mean will approximate a normal distribution as long as the sample size is `sufficiently large`. 
## 5. How large does the sample size need to be for the normal approximation to occur?
- The larger the sample size, the more closely the sampling distribution of the sample mean will follow a normal distribution.
- Typically, we consider a sample size of `30 to be sufficiently large`.
-	If the sample size is less than 30, the central limit theorem doesn’t work anymore. The sampling distribution of the sample mean will follow normal distribution only if the population distribution is also normal.
-	If the sample size is greater than 30, the central limit theorem applies and the sampling distribution will follow normal distribution regardless of the population distribution. However, `a strongly skewed distribution requires a larger sample size`.
## 6. How does sample size affect the sampling distribution of the mean?
As the sample size (n) increases, the denominator of the formula becomes bigger, then the SEM (standard error of the mean) becomes smaller, the sampling distribution becomes tighter, and the more precise the sample mean can be used to estimate the population mean.
## 7. Why Central Limit Theorem is Important?
1. The normality assumption:
- In real-world data, it is common to have outliers, skewness, and asymmetry. 
- Many statistical practices, such as, hypothesis tests, confidence intervals, and t-tests are based on the normality assumption. 
- The use of appropriate sample size and the Central Limit Theorem helps us to get around the problem of non-normality in the data.
2. The precision of estimates:
- In practice, we typically only have ONE set of random samples. 
- We often use statistical inference to estimate population parameters (e.g., population mean) using sample statistics (e.g., the sample mean). 
- The sample mean is the Best linear unbiased estimator (BLUE) of the population mean. 
- However, it is not good enough to use the point estimate (e.g., the sample mean) to infer the population mean because it will almost always be off the mark.
- `If we were to take random samples over and over again and compute the mean of all these sample means. It will be a very good estimate of the population mean`. 

------------------------
# Understanding Boxplot: Infinity Gauntlet of the Dataverse
(Use boxplots and Tukey’s Method to eliminate outliers in a snap of your fingers (or code))

The power of summarizing huge amounts of data is condensed into just 6 values (Boxplots represent these 6 values visually).
<p align="center">
  <img src="https://github.com/akimwong/akimwong/blob/main/articles/summaries/statistics/boxplot1.png" width="600" height="500">
</p>

Using them you can:
- Get a great sense of numeric data
- Do a quick graphical examination
- Compare different groups within the data
- Use them to know and eliminate outliers from the data
<p align="center">
  <img src="https://github.com/akimwong/akimwong/blob/main/articles/summaries/statistics/boxplot2.png" width="600" height="300">
</p>

1.	The `Minimum`, is the smallest value in the list, 1 in this case.
2.	The `Maximum` is the largest value, i.e. 100.
3.	The `Median` is the number right in the dead center of the list. 50% of the data lies on each side of the median. 40 is in the middle of the above list (is itself also called the second quartile or Q2).
4.	There’s also the `Mean`, which is in the middle too. But not the middle of the list, but rather in the arithmetic middle of the values in the list, it is a sum of all values divided by the count of values in the list, which is 40.8 in this case.
5. The `First Quartile (or Q1)` is the value under which 25% of the data points lie. In a sense, it is `the median of the first half` of the data.
6. The `Third Quartile (or Q3)` is the value under which 75% of the data points lie. It is `the median of the second half` of the data.
7. `Inter Quartile Range (IQR)` is the difference between the third quartile and the first quartile: (Q3 — Q1). It gives the range of the middle half of the data.
8. The `T-shapes protrusions` on either side of the box are called whiskers or fences. They fence off the relevant data from the outliers.
- The Lower Fence is calculated as Q1 — (1.5 * IQR)
- The Upper Fence is calculated as Q3 + (1.5 * IQR)

Why the separation is 1.5 times the IQR on either side? the answer lies in statistics.  According to the 68–95–99.7 rule, most of the data (99.7%) lies within 3 standard deviations ( <3σ ) from the mean on either side of a standard distribution. Everything outside it is an outlier.

### Tukey’s method is used to remove outliers
<p align="center">
  <img src="https://github.com/akimwong/akimwong/blob/main/articles/summaries/statistics/GetOutliersPython1.PNG" width="600" height="300">
</p>
<p align="center">
  <img src="https://github.com/akimwong/akimwong/blob/main/articles/summaries/statistics/GetOutliersPython2.PNG" width="600" height="150">
</p>

----------------------
# Data Scientists Need to Know Just One Statistical Test
(After you read this, you will be able to test any possible statistical hypothesis. With a unique algorithm.)

### There is only one test that you need to know because `all the statistical tests are in reality the same one test!`
- And once you really grasp how this one test work, you will be able to test any hypothesis you will ever need.

### What is the profound meaning of any statistical test?
- You have a hypothesis (called “null hypothesis”) and you want to put it to the test. Thus, you ask yourself: “If the hypothesis was true, `how often` would I get an outcome as suspect as the outcome that I actually had?”
- In statistics, this “how often” is called “p-value”.
- At this point, the line of reasoning is pretty trivial: if the p-value is very low, then it means that your original hypothesis is likely to be wrong.
- Note that the concept of “unexpectedness” depends closely on the specific hypothesis that you are testing. 

### The ingredients of statistical testing
Reading the previous paragraph, you may have guessed that we need two ingredients:
1.	The distribution of the possible outcomes, depending on the null hypothesis.
- It’s not always straightforward to get the full distribution of outcomes. 
- Often, it’s more convenient (and easier) to randomly simulate a high number of outcomes: this is a good approximation of the true distribution.
3.	A measure of the “unexpectedness” of any outcome.
- We need to define a function that maps each possible outcome into a single number. 
- This number must express how unexpected the outcome is, provided that the null hypothesis is true: the more unexpected the outcome, the higher this score.

Once we have these two ingredients, the job is basically done. In fact, it’s enough to calculate the unexpectedness score of each outcome in the distribution and the unexpectedness score of the observed outcome.

### The p-value is the percentage of random scores that are higher than the observed score


### A unique statistical test


### So why all those statistical tests?
- If you have come this far, you may wonder: if it’s so easy, why do so many tests exist? The answer is mostly “historical”.
- There was a time when computation was much more expensive than now, so “statistical tests” were basically shortcuts to compute p-values efficiently. 
- And since there are so many possibilities to choose step 1 and step 2 of the algorithm we have seen, the tests proliferated.
