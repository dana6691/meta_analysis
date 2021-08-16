# meta_analysis
A statistical method that combines the results of several trials to generate an average result. 

# Process
1. Frame a quation using **PICO**(Participant, Intervention, Comparisons, Outomces)
2. Literature search and select papers using PRISMA diagram
3. Conduct Heterogeneous test and select the statistical models
4. Estimate the summary effect size and construct a forest plot
5. Determine the extent to which these articles have publication bias and run multiple funnel plots
6. Find moderator variables and conduct subgroup analyses and meta regression to test if there are subsets of research that capture the summary effects 

# Heterogeneity test 
H0: the variation in study outcomes between studies.

- Q (Cochran, 1954) 
calculated as the weighted sum of squared differences between individual study effects 
Has lower power if the number of studies is small
- I^2 (Higgins & Thompson, 2002) tests
I² statistic describes the percentage of variation across studies = 100% x (Q-df)/Q
I² will be low = very little variation between trials= fixed effects model might be appropriate
