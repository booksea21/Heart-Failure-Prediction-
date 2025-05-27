# Heart-Failure-Prediction-
Heart Failure Clinical Data Analysis
This project performs a comprehensive statistical analysis on the [Heart Failure Clinical Records Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records). Using Python and various statistical tools, it explores the relationships between patient health attributes and death events, helping to identify potential risk factors.
**Dataset**
The dataset contains clinical records of 299 patients who experienced heart failure. It includes 13 features such as:
- Age, Anaemia, Creatinine Phosphokinase, Diabetes, Ejection Fraction
- High Blood Pressure, Platelets, Serum Creatinine, Serum Sodium
- Sex, Smoking, Time (follow-up period), and Death Event (target)
 Libraries Used
pandas, numpy, matplotlib, seaborn, plotly, scipy.stats, forestplot
**Statistical Tests Conducted**
1.  Mann-Whitney U Test (Non-parametric)
To compare distribution differences in:
- High Blood Pressure vs Death Event
- Platelet Count vs Death Event

**Results:**
HBP: p-value = 0.1710 → Not Significant
Platelets: p-value = 0.4255 → Not Significant

**Conclusion:** 
No statistically significant distribution difference. Null hypothesis not rejected.
* 2. Chi-Square Test (Association)
Tested categorical features against DEATH_EVENT:
- Feature	χ² Statistic	P-Value	Conclusion
- High BP	1.54	0.214	❌ No significant association
- Smoking	0.0073	0.9317	❌ No significant association
- Gender	0.0000	1.0000	❌ No significant association
- Anaemia	1.04	0.307	❌ No significant association
- Diabetes	0.0000	1.0000	❌ No significant association
* 3. Odds Ratio & Forest Plot
Estimated Odds Ratios and Confidence Intervals:
- Variable	Odds Ratio	95% CI Lower	95% CI Upper
- Smoking	0.94	0.54	1.64
- Gender	0.98	0.57	1.69
- Anaemia	1.33	0.79	2.23
- Diabetes	0.99	0.59	1.67
- Interpretation: None of the odds ratios are statistically significant (CI includes 1).
* Visualizations
- Histogram of Serum Sodium by Death Event
- Q-Q Plots for Age Distribution (Alive vs Dead patients)
**Insights**
No individual variable (including high blood pressure, diabetes, or smoking) showed strong statistical association with death events.
Future work may involve multivariate analysis, logistic regression, or machine learning models for better insights.
 
