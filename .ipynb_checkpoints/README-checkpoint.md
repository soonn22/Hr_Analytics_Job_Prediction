# Overview
I am tasked with analyzing employee turnover at Salifort Motors using Python for model building and data analysis as a part of Advanced Google Data Analysis capstone project. The company is experiencing high turnover rates, and leadership wants to understand the key drivers behind employee departures to improve retention and reduce costs.
I will work with survey data and build predictive models to determine whether an employee is likely to leave the company. Logistic regression or machine learning models such as decision tree, random forest, and XGBoost will be built after this prject. My goal is to evaluate different models and provide insights into factors influencing turnover.
In addition to developing a strong predictive model, I will need to communicate findings effectively by preparing an executive summary that presents key takeaways and recommendations to stakeholders.

# EDA Summary
1. Project Load & Work Hours: Employees with 3-4 projects and working between 160-220 hours per month have the lowest turnover rate(22%). voerburdened employees(more than 4 projects) and underworked employees(fewer than 160 hours) show higher turnover(78%). Redistribution of tasks can improve retention.
2. Satisfaction-toEvaluation Ratio: Maintaining a raito above 1 reduces turnover. Lower-income employees tend to have lower ratios, and long working hours without proper compensation negatively impact satisfaction levels.
3. Salary & Working Hours: Employees working ove 275 hours without sufficient pay show dissatisfaction and higher turnover risk. Meanwhile, employees working fewer than 125 hours exhibit unstable satisfaction levels, which can be improved with increase workload and salaries.
4. Promotion impact: Employees who received promotions in the last 5 years have a significantly lower turnover rate (5.96%) compared to non-promoted employees(24.2%). Increasing promotion rates can improve retention.
   



# Building predictive model

I have found important feature to develop predictive models from explanatory data analysis. the purpose of this project is to find key features affecting on high turnover rate and the leadership would like to reduce cost of employees turnover. The next challenge for this project is to develop predictive model.

1. naive bayesian model
2. decision trees
4. random forest model
5. xgboost model
## Features

Target values : 'left'
Predictors : 'number_project', 'average_monthly_hours', 'salary', 'sat/eval', 'year_spent_ratio', 'promotion_last_5years'

After testing Gaussian Naïve Bayes, Decision Tree, Random Forest, and XGBoost, the Random Forest model emerged as the best performer, achieving the highest F1-score of approximately 96%, indicating high reliability in predictions.
By leveraging cross-validation techniques, the model's accuracy was optimized, ensuring robust performance across different data splits. With this powerful predictive capability, leadership can proactively identify employees at risk of leaving the company, allowing them to make informed decisions based on key model features.

# Model application
The company has employee data. enter these data into the model and predict which employee will leave the company soon. Understanding those employees will give insight for strategic plan to reduce turnover rate.  



# Next steps

## Strategic plan (suggestions)
Satisfaction level, last evaluation, promotion last 5 years, number of project, average monthly work hours and salary are key features for high turnover rate as confirmed in explanatry data analysis.
There are tree approach to improve employee turn over.
1. Optimization of workload
   - 3-4 projects and 160-220 work hours per month in average is the opimal workloads.
   - Assign more tasks and projects to employees with under optimal workloads
   - Assign less tasks and projects to employees with over optimal workloads
2. compensation
   - low and medium salary gourps of employee with over 275 works hours receive insufficient compensations for their efforts
   - Investigate reasons of insufficient compensations.
   - Provide free or paid training programs to employees with low evaluation score to improve their performance.
3. promotion
   - Employees without promotion leave the company.
   - build career developing program in company and support employees to achieve and give more chance to existing employees.

## collecting data and evaluation the performance
1. Collecting data of employees and costs
   - Collect employee data who has experiences strategic plan and analyze employee data
   - calcualte costs of strategic plan and turn over rates.
   - calcuate saved cost by reducing turnover rates.
   - compare cost and saving to adjust strategic plan.

