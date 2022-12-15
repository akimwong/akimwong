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





Using them you can:
- Get a great sense of numeric data
- Do a quick graphical examination
- Compare different groups within the data
- Use them to know and eliminate outliers from the data




