# ML_project_CustomerPropensityToPurchase
The identification of factors and online behaviors that influence customers to abandon their shopping carts on the store's website.

---

Data: [Customer Propensity to Purchase Data](https://www.kaggle.com/datasets/benpowis/customer-propensity-to-purchase-data)

Goal: Analyze whether a given customer will make a purchase with us or not.

Stakeholder: An online store owner aiming to minimize the risk of abandoned shopping carts.

---




![image](https://github.com/user-attachments/assets/835ee4f3-4307-4bed-98fc-9f1fa6d62a49)


![image](https://github.com/user-attachments/assets/44fce770-43b3-47ec-8077-84b6998c7aee)



ML_Project_CustomerPropensityToPurchase

The identification of factors and online behaviors that influence customers to abandon their shopping carts on the store's website.

Project Overview

Data

Dataset: Customer Propensity to Purchase Data

Description: The dataset contains information about buyer interactions, representing a single day’s activity on a fictional e-commerce website. It includes:

Over 455,000 rows associated with unique user IDs.

23 columns describing features of user visits and actions on the site over the course of one day.

Goal

Analyze whether a given customer will make a purchase and identify the key factors and behaviors that lead to cart abandonment. This will help recommend strategies to increase the likelihood of items being added to the cart and, eventually, finalized purchases.

Stakeholder

An online store owner aiming to minimize the risk of abandoned shopping carts and maximize conversion rates.

Project Steps

Four notebooks were prepared to guide the analysis and modeling:

00_Data_Preparation_and_Cleanup:

Cleaning and preprocessing the dataset to ensure quality and usability for analysis and modeling.

01_Exploratory_Data_Analysis (EDA):

Conducting general statistical analysis to understand user behaviors and identify trends or patterns.

02_Logistic_Regression_Analysis:

Using logistic regression to analyze the factors influencing users to add items to their carts.

03_XGBoost_Analysis:

Applying the XGBoost algorithm to identify factors influencing cart additions, with hyperparameter tuning and SHAP analysis for interpretability.

Observations and Insights

Statistical Insights:

User Activity: Half of the users did not perform any actions on the site.

Purchase Conversion Rate: Only 4% of users completed a purchase.

Geographical Data: The majority (93%) of users accessed the site from the United Kingdom.

Device Usage: The store was accessed primarily via mobile devices, more than three times as often as tablets or computers.

Returning Customers: Over half of the users were returning customers.

Behavioral Patterns:

Non-Purchasing Users: The top 10 most frequent actions, during which no purchases were made, accounted for 39% of all records. These include:

Accessing the homepage.

Using a dropdown menu to view products.

Mobile access by returning customers.

Purchasing Users: The top 10 most frequent actions that resulted in purchases accounted for 2% of all records. These patterns include:

Adding items to the cart.

Logging in.

Viewing the order summary.

All purchasing users used smartphones, whereas 15% of non-purchasers used a tablet or computer.

Key Modeling Results

Logistic Regression:

Baseline Dataset Accuracy:

Training set: 61%

Test set: 61%

True Positive Rate: 43%

After Cleaning Irrelevant Actions:

Training set: 75%

Test set: 75%

True Positive Rate: 74%

XGBoost:

After Cleaning and Hyperparameter Tuning:

Accuracy: 77%

True Positive Rate: 76%

SHAP analysis was used to interpret the model’s results.

Recommendations

Since only 4% of users who add items to their cart finalize their purchase, increasing the number of cart additions could potentially boost sales. Insights and actionable recommendations include:

Key Factors Influencing Cart Additions:

Users visiting the homepage.

Using dropdown menus to explore products.

Checking delivery information on product pages.

Targeted Actions:

Enhance the user experience on mobile devices, as they dominate purchasing behaviors.

Improve visibility and usability of product exploration features, such as dropdown menus.

Streamline the process of accessing delivery information to encourage cart additions.

Engagement Strategies:

Focus on returning customers, as they are more likely to complete purchases.

Create targeted promotions or reminders to re-engage users who have previously added items to their carts.

Conclusion

The project has identified key factors and behaviors influencing cart additions and purchases, providing actionable insights to help reduce cart abandonment rates and improve overall conversion rates.

