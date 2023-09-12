# Proportion Testing Project Overview
The project consists of a split test analysis between male and female voters.

# Objectives
- Estimate Sample Statistics
- Visualize Sampling Distributions
- Perform Hypothesis Test

# Results
Male Voter Statistics:

- Male Voters: 642

- Sample Size: 1000

- Proportion of Male Voters: 0.642

- Variance of Male Voters: 0.0002298

- Standard Deviation of Male Voters: 0.0151603

---

Female Voter Statistics:

- Female Voters: 591

- Sample Size: 1000

- Proportion of Female Voters: 0.591

- Variance of Female Voters: 0.0002417

- Standard Deviation of Female Voters: 0.0155473

---

## Sampling Distributions
![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/f355ab8d-473c-440d-87b1-7bfdb914f913)

- Difference in Sample Proportions: 0.051

- 95% Confidence Interval for the Sample Proportions: 0.008 to 0.094.
![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/c5a1c605-2c46-465c-81ad-fbd1463e12a7)

---

## Hypothesis Testing
Null Hypothesis: 

- No Difference in Proporitons
- Proportion of Male Voters - Proportion of Female Voters = 0
- Therefore, Proportion of Male Voters = Proportion of Female Voters.

Alternative Hypothesis: 

- A Difference Exists
- Proportion of Male Voters != Proportion of Female Voters
- Therefore, Proportion of Male Voters - Proportion of Female Voters != 0  

Significance level: 5%

Assuming the Null Hypothesis is Correct:

- Sampling Proportion: 0.6165

- Standard Deviation for Sampling Proportion of Male & Female Voters: 0.0217

- Z-Score for Sampling Difference Between Male & Female Voters: 2.35

![image](https://github.com/frantzalexander/proportion_testing/assets/128331579/0452a16c-420b-4eda-bf0a-61984a9071ab)

## Conclusion:
- Calculated P-Value of 0.019 is Below the Significance Level of 5%.

Therefore, We Reject the Null Hypothesis.
- There Exists A Significant Difference in the Proportion of Male & Female Voters. 



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
samp
sampling2[Visualize Proportion Difference Sampling Distribution]
start --> calculate
calculate -->|Male Proportion Analysis|male_proportion
male_proportion --> male_var
male_var --> male_std
male_std --> sampling
calculate --> |Female Proportion Analysis|female_proportion
female_proportion --> female_var
female_var --> female_std
female_std --> sampling
