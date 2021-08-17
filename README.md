# Meta Analysis
A statistical method that combines the results of several trials to generate an average result. 

1. Frame a quation using **PICO**(Participant, Intervention, Comparisons, Outomces)
2. Literature search and select papers using PRISMA diagram
3. Conduct Heterogeneous test and select the statistical models
4. Estimate the summary effect size and construct a forest plot
5. Determine the extent to which these articles have publication bias and run multiple funnel plots
6. Find moderator variables and conduct subgroup analyses and meta regression to test if there are subsets of research that capture the summary effects 

## Heterogeneity test 
H0: the variation in study outcomes between studies.

- **Q (Cochran, 1954) test** calculated as the weighted sum of squared differences between individual study effects. Has lower power if the number of studies is small

-  **I^2 (Higgins & Thompson, 2002) test** describes the percentage of variation across studies = 100% x (Q-df)/Q. 
I² will be low = very little variation between trials= fixed effects model might be appropriate

## Statistical models
- Fixed model = consider all trials as one trial. 
If Q test is not significant and I² will be low, use fixed model

- Mixed model = fixed + random effect.
Use if there’s anything different, ages, locations or people who performed each trial.
= true effect size may or may not vary from study to study

## Effect size
- Dichotomous data
  - computation of the **log(RR)** or the **log(OR)**, or the **RD**
  - not easily interpretable. 
  - ex) each individual study may be used or the number of events and the total number of participants for each group. RR and RD may be computed for any experimental study (RCT) or quasi-experimental study or cohort studies.

- Continuous data
  -  **mean difference (MD)/weighted mean difference (WMD)** Computation the difference in means from each individual study are used. It is used if all studies included in meta-analyses measured the outcome using the same measurement instrument. The results are expressed in the natural (clinical) units used for the common measurement instrument. 
        -  reviewers provide explanations regarding the interpretation of the results expressed in units used for the common measurement instrument. The minimum score and the maximum score.
        -  Also, should specify what change (difference) is considered significant from a practical or clinical point of view. 
        -  should explain the interpretation of a negative or positive difference. 
  - **standardized mean difference (SMD)**: is a difference in means that is standardized by using information on the variability of data (standard deviation). Use if the studies measured the same outcome but with different measurement instruments.
      - 3 computation methods: *'Cohen’s d, Hedges’ adjusted g, and Glass’s delta'*. 
      - For meta-analysis computation the SMD from each individual study are used. The results are expressed in units of standard deviation.
      - It is recommended that reviewer’s convert the results into natural (clinical) units by multiplying the results expressed in units of standard deviation with the standard deviation of the scores from a study on a known measurement instrument. 

*risk ratio (RR) <br>
*risk difference (RD) <br>
*odds ratio (OR)<br>

### SMD Effect Size
- Cohen’s d
- Hedges’ adjusted g
  -  less than 0.2 = small effect, >0.5 = medium, >0.8 = large effect
  - Close to 0, there’s no significant difference between groups.
  - If CI of SMD includes 0, is not statistically significant.
  - *but <0.2 effect should not be necessarily rejected as a inconsequent. If the sample is large, the small difference can be significantly difference. 
  
### Measuring Effect Size
- Forest Plot
  - Plot each outcome
  - conventional meta-analysis approaches using study-level log(OR) 
  - Summary effect measures, such as a pooled odds ratios

## Analysis the source of between-studies variation
- **Subgroup analysis**: it assumes that all studies within a subgroup share a common effect size.
- **Meta-Regression**: it assumes that all studies which have the same values on the covariates share a common effect size.

## Advanced Model
- Subgroup Analysis
- Meta-Regression Analysis
- Multilevel Meta-Analysis
- Meta-Analytics structural equation modeling
- Network Meta-Analysis
- Bayesian Meta-Analysis

Reference: Harrer, M., Cuijpers, P., Furukawa, T.A., & Ebert, D.D. (2021). Doing Meta-Analysis with R: A Hands-On Guide. Boca Raton, FL and London: Chapmann & Hall/CRC Press. ISBN 978-0-367-61007-4.
