# Salifort Motors employee churn project

 # Project overview
 Employee data was collected from Salifort Motors to understand why employees churned and what can be done to improve their conditions and satisfaction.

# Business Understanding
 
Employees at Salifort Motors had a high rate of turnover. This turnover was concerning for Salifort because they pride themselves on haveing a workplace that supports employee success and professional development.
Additionally, training at Salifort is costly- every employee requires recruitment, training and development. Increasing tenure can save the compant costs. The goal of the project is to gather metrics about employee
performance and satisfaction to derive factors that correlate with churn and make recomendations for improvement.

# Data Understanding

The data gathered for each employee was: Satisfaction score from a survey, their last performance review score, the number of projects the employee works on, their average monthly hours worked, whether they had an accident in the workplace, whether the had a promotion in the last 5 years, their salary level, their department, and whether or not they left.

![image](https://github.com/salto571/Salifort-Motors/assets/17547391/79f529ab-1541-42c9-84a3-ef43390efeb9)

![image](https://github.com/salto571/Salifort-Motors/assets/17547391/bf34f48d-5d49-4cdf-8fcf-b1dbd00aa80c)

# Modeling and Evaluation

Two models were built: a random forest and a boosted model. Both models were built using a cross validated grid search optimized for recall, with employment status as the dependent variable. Recall was selected because the it was more important to buikd a model that correctly identifies as many employees who churned as possible with some false positives being acceptable, rather than building a modeloptimized on precision that has higher false negatives. Nevertheless, the models were built incorporating accuracy, precision, recall, and f1 scores. During the EDA phase it was determined that the department and workplace accident variables were poorly correlated with tenure and were dropped from the models. 

The boosted model had a recall of 0.925 compared the the random forest's score of 0.916 and thus was selected.

# Conclusion

It is clear that employees who are overworked are more likely to leave. Recommendations: 1) Give employees a cut off for how many hours they are allowed to work OR make sure they are well compensated for overtime 2) Make sure that if they are working on too many projects (4 or more) that they are given the support staff or help they need. 3) Make sure they are not feeling alone or swamped. 4) For employees who were with the company a long time(5 or more years), consider a pay increase, title upgrade, bonus, or other benefit. If management thinks the employee performance indicates that they should not get one of these benefits, meet with the management and the employee to come up with a decision on continuing employement, goals, and performance objectives
