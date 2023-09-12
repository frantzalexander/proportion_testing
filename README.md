# Proportion Testing Project Overview
The project consists of a split test analysis between male and female voters.

# Objectives
- Estimate sample statistics
- Visualize sampling distributions
- Perform hypothesis test

# Results
Male Voter Statistics:

- Male voters: 642

- Sample size: 1000

- Proportion of male voters: 0.642

- Variance of male voters: 0.0002298

- Standard deviation of male voters: 0.0151603

---

Female Voter Statistics:

- Female voters: 591

- Sample size: 1000

- Proportion of female voters: 0.591

- Variance of female voters: 0.0002417

- Standard deviation of female voters: 0.0155473

---

## Sampling Distributions
![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/f355ab8d-473c-440d-87b1-7bfdb914f913)

- Difference in sample proportions: 0.051

- 95% confidence interval for the sample proportions: 0.008 to 0.094.
![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/c5a1c605-2c46-465c-81ad-fbd1463e12a7)

---

## Hypothesis Testing
Null Hypothesis: 

- No difference in proportions
- Proportion of male voters - proportion of female voters = 0
- Therefore, proportion of male voters = proportion of female voters.

Alternative Hypothesis: 

- A difference exists
- Proportion of male voters != proportion of female voters
- Therefore, proportion of male voters - proportion of female voters != 0  

Significance level: 5%

Assuming the null hypothesis is correct:

- Sampling proportion: 0.6165

- Standard deviation for sampling proportion of male & female voters: 0.0217

- Z-Score for sampling difference between male & female voters: 2.35

![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/45699511-3c30-4f89-82e3-b6566019faeb)

---

## Conclusion
- Calculated P-Value of 0.019 is below the significance level of 5%.

Therefore, we reject the null hypothesis.

Assume a significant difference in the proportion of male & female voters. 



# Process
```mermaid
flowchart TD 
start(((START)))
calculate{Calculate Voter Sample Statistics}
male_proportion[Male Voter Proportion]
male_var[Male Voter Proportion Variance]
male_std[Male Voter Proportion Standard Deviation]
female_proportion[Female Voter Proportion]
female_var[Female Proportion Variance]
female_std[Female Voter Proportion Standard Deviation]
sampling[Visualize Sampling Distributions]
cal1[Calculate Sample Proportion Difference Statistics]
cal2[Sample Porportion Difference]
sigma[Sample Proportion Difference Standard Deviation]
confidence[Calculate Confidence Interval]
sampling2[Visualize Proportion Difference Sampling Distribution]
null[Calculate Null Hypothesis Statistics]
critical[Critical Values]
threshold[Upper & Lower Thresholds]
visualize[Visualize Distribution PDF]
finish(((END)))
start --> calculate
calculate -->|Male Proportion Analysis|male_proportion
male_proportion --> male_var
male_var --> male_std
male_std --> sampling
calculate --> |Female Proportion Analysis|female_proportion
female_proportion --> female_var
female_var --> female_std
female_std --> sampling
sampling -->cal1
cal1 --> cal2
cal2--> sigma
sigma --> confidence
confidence --> sampling2
sampling2 --> null
null --> critical
critical --> threshold
threshold --> visualize
visualize --> finish

