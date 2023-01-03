# Final Project Absolute (Banking Marketing Targets)
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

# Bank Client Data
1. age (numeric)

2. job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')

3. marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)

4. education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')

5. default: has credit in default? (categorical: 'no','yes','unknown')

6. housing: has housing loan? (categorical: 'no','yes','unknown')

7. loan: has personal loan? (categorical: 'no','yes','unknown')

8. balance: average yearly balance, in euros (numeric)


# Related with the last contact of the current campaign
9. contact: contact communication type (categorical: 'cellular','telephone')

10. month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')

11. day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')

12. duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.


# Other attributes
13. campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)

14. pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)

15. previous: number of contacts performed before this campaign and for this client (numeric)

16. poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')


# Stage 0 - Project Background
Stage 0 is an early stage where we implemented 'ask' in data life cycle. There are details about our role, problem statement, goal, objective and business metrics of our project.

# Stage 1 - Exploratory Data Analysis
Stage 1 is a next step that we focused on gathering insights from statistical views.

What we have done on this stage:

-Descriptive Analysis

-Univariate Analysis

-Multivariate Analysis

-Business Insight As Business Recommendation

# Stage 2 - Preprocessing Data
Stage 2 is another next step that we did manipulation on data before it is used in order to build the model.

What we have done on this stage:

-Handle Missing Values

-Handle Duplicated Data

-Handle Outliers

-Feature Transformation

-Feature Encoding

-Handle Class Imbalance

-Feature Selection

-Feature Extraction


# Stage 3 - Modeling and Evaluation
Stage 3 is a step where we tested our data train to machine learning model and evaluated it. On this stage we created 7 different preprocessing treatment on datasets. We tested it to 5 different models: logistic regression, decision tree, random forest, XGBoost and AdaBoost. The objective of it's action is at the end of this stage we couldn't only know which the better model also the better preprocessing treatment on dataset. As we know, in data science everything is experimental, so we did it to get the better result.

What we have done on this stage:

-Preprocessing Data

-Splitting Data (Data Train and Data Test)

-Feature Engineering

-Model Testing

-Tuning Hyperparameters and feature selection

-Model Selection

-Evaluation most impacful/influence to model output using shap library


# Stage 4 - Final Presentation Material
Based on our project's result, out best model is AdaBoost with accuracy score 90% and precision score 55%. Our model performance could increase deposito subscribe rate  by 0.87x.
