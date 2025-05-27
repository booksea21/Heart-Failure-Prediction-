# Heart-Failure-Prediction-
This project looks at health data from people who had heart failure, to see which health conditions might be connected to whether a person survives or not. We use statistics to ask and answer questions like:
- Does having high blood pressure increase your chance of death?
- Are people with diabetes more likely to die from heart failure?
- Do blood test results show a pattern in who lives and who doesn’t?
What’s in the Data?
We have information from 299 people. For each person, we know things like:
- Their age and gender
- Whether they have conditions like anaemia, diabetes, or high blood pressure
- Results from blood tests
- Whether they were smoking or not
- And most importantly: whether they died (1) or survived (0)
**What Did We Test?**
1. Are there differences between those who died and those who survived?
We used a test called the 'Mann-Whitney U Test' to compare things like high blood pressure and blood platelet count. The goal: see if these values look very different for people who died versus those who survived.

Result: There was no strong evidence that high blood pressure or platelet count were clearly different between the two groups.
2. Are any conditions clearly linked to death?
We used another test called the 'Chi-Square Test'. It helps us check if there’s a relationship between two things.
For example: Are people with anaemia more likely to die?

Result: Again, we didn’t find strong evidence that things like smoking, diabetes, or anaemia are clearly linked to death.
3. What about risk levels?
We calculated something called 'odds ratios' to see how much more (or less) likely death is when a person has a condition.
An odds ratio above 1 = more risk. Below 1 = less risk.

 Result: None of the conditions showed a strong or clear effect.
**What Do the Graphs Show?**
- We looked at blood sodium levels with a bar chart to compare survivors and non-survivors
- We also checked if people’s ages followed a normal pattern using something called a Q-Q plot
 Final Takeaway
Although we looked at many health features, we didn’t find any one feature that strongly predicts death from heart failure by itself. This means we may need to look at combinations of features together, or use more advanced tools like machine learning to find deeper patterns.
Data Source
This data came from a trusted public source: the UCI Machine Learning Repository.



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
 <img width="907" alt="Screen Shot 2025-05-27 at 07 27 57" src="https://github.com/user-attachments/assets/bc163b55-ecb3-4169-9919-aa51bd6063f6" />
 <img width="690" alt="Screen Shot 2025-05-27 at 07 28 45" src="https://github.com/user-attachments/assets/01f3f8dd-871c-4ffd-8349-050f6ce54e32" />
<img width="476" alt="Screen Shot 2025-05-27 at 07 30 23" src="https://github.com/user-attachments/assets/fb8832c1-e613-4121-969a-ca618c4c81cf" />
<img width="712" alt="Screen Shot 2025-05-27 at 07 30 56" src="https://github.com/user-attachments/assets/1f47da1a-9c47-4cbc-8307-678dfff64ed3" />
<img width="707" alt="Screen Shot 2025-05-27 at 07 32 02" src="https://github.com/user-attachments/assets/f17209ec-d32a-4a8c-aab2-4aa55e55f9d6" />
