# Proportion Testing Project Overview
The project consists of a split test analysis between male and female voters.

# Objectives
- Estimate Sample Statistics
- Visualize Sampling Distributions
- Perform Hypothesis Test

# Results
Male Voter Statistics

Male Voters: 642

Sample Size: 1000

Proportion of Male Voters: 0.642

Variance of Male Voters: 0.0002298

Standard Deviation of Male Voters: 0.0151603

---

Female Voter Statistics

Female Voters: 591

Sample Size: 1000

Proportion of Female Voters: 0.591

Variance of Female Voters: 0.0002417

Standard Deviation of Female Voters: 0.0155473

---

## Sampling Distributions
![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/f355ab8d-473c-440d-87b1-7bfdb914f913)

The difference in sample proportions: 0.051

The 95% confidence interval for the sample proportions is between: 0.008 to 0.094.
![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/c5a1c605-2c46-465c-81ad-fbd1463e12a7)

---

## Hypothesis Testing
Null Hypothesis: 

- There is no difference
- Where the proportion of male voters - proportion of female voters = 0
- Therefore, the proportion of male voters = proportion of female voters.

Alternative Hypothesis: 

- There is a difference
- Where the proportion of male voters != proportion of female voters
- Therefore the proportion of male voters - the proportion of female voters != 0  

Significance level: 5%

Assuming the Null Hypothesis is correct:

The sampling proportion: 0.6165

The standard deviation for the sampling proportion of male & female voters: 0.0217

The Z-Score for the sampling difference between male and female voters: 2.35

![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/0452a16c-420b-4eda-bf0a-61984a9071ab)

## Conclusion:
The calculated p-value of 0.019 is below the set significance level of 5%.

Therefore, we reject the null hypothesis and accept the alternative. 

There is a significant difference in the proportion of male and female voters.

# Process
```mermaid
flowchart TD 
start(((START)))
calculate[Calculate Sample Statistics]
