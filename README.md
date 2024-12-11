# Machine Learning Customer Propensity to Purchase

**!! This project is made in Polish because of the Polish bootcamp.**


This project was completed as part of a DataScience Bootcamp. Our team, called **RocketScience Team**, consisted of three members. The goal of the project was to analyze customer behaviors and interactions on a fictional e-commerce website to understand the factors influencing cart abandonment and purchase conversions. By identifying these key behaviors, we aimed to provide actionable insights that would increase purchase likelihood and reduce cart abandonment rates.

## Project Overview

### Data

Data: [Customer Propensity to Purchase Data](https://www.kaggle.com/datasets/benpowis/customer-propensity-to-purchase-data)

The dataset contains information about buyer interactions, representing a single day's activity on an e-commerce website. It includes:

- Over 455,000 rows of data associated with unique user IDs.
- 23 columns describing features of user visits and actions on the site over the course of one day.

### Goal

- Analyze whether a given customer will make a purchase.
- Identify the key factors and behaviors that lead to cart abandonment.
- Provide recommendations to increase the likelihood of items being added to the cart and, eventually, finalized purchases.

### Stakeholder

An online store owner aiming to minimize the risk of abandoned shopping carts and maximize conversion rates.

## Project Parts

### 1. Data Preparation and Cleanup (`01_Data_Preparation_and_Cleanup`)

- Clean and preprocess the dataset to ensure quality and usability for analysis and modeling.

### 2. Exploratory Data Analysis (EDA) (`02_Exploratory_Data_Analysis`)

- Conduct general statistical analysis to understand user behaviors and identify trends or patterns.

### 3. Logistic Regression Analysis (`03_Logistic_Regression_Analysis`)

- Use logistic regression to analyze the factors influencing users to add items to their carts.

### 4. XGBoost Analysis (`04_XGBoost_Analysis`)

- Apply the XGBoost algorithm to identify factors influencing cart additions.
- Perform hyperparameter tuning and SHAP analysis for model interpretability.

## My Contribution

As part of the **RocketScience Team**, my primary focus was on the **statistical analysis** of user behavior and exploring the question: *What actions do people take before they add items to their shopping cart?*

Given that only 4% of users who added items to their cart completed their purchases, I focused on understanding what could potentially increase the frequency of cart additions. I hypothesized that improving the actions that lead up to adding products to the cart could lead to an increase in overall sales.

### Key Areas I Focused On:
- **Identifying user behaviors before cart additions**: I analyzed the data to understand the sequence of actions users take before adding items to their baskets.
- **Statistical insights**: I worked on exploring trends and patterns in user activity to identify what may lead to cart additions and, ultimately, to purchases.
- **Behavioral patterns**: I helped pinpoint the most common actions (e.g., using dropdown menus, viewing delivery information) that are associated with cart additions.

By identifying these factors, we can focus on improving the overall shopping experience, encouraging more users to add items to their carts, thus increasing the chances of finalizing the purchase.

## Observations and Insights

### Statistical Insights

- **User Activity**: Half of the users did not perform any actions on the site.
- **Purchase Conversion Rate**: Only 4% of users completed a purchase.
- **Geographical Data**: The majority (93%) of users accessed the site from the United Kingdom.
- **Device Usage**: The store was accessed primarily via mobile devices, more than three times as often as tablets or computers.
- **Returning Customers**: Over half of the users were returning customers.

### Behavioral Patterns

- **Non-Purchasing Users**: The top 10 most frequent actions (such as accessing the homepage, using the dropdown menu to view products, and mobile access by returning customers) accounted for 39% of all records where no purchase was made.
- **Purchasing Users**: The top 10 most frequent actions (such as adding items to the cart, logging in, and viewing the order summary) accounted for only 2% of all records, but these actions led to purchases.
  - All purchasing users used smartphones, whereas 15% of non-purchasers used a tablet or computer.

## Key Modeling Results

### Logistic Regression

- **Baseline Dataset Accuracy**:
  - Training set: 61%
  - Test set: 61%
  - True Positive Rate: 43%

- **After Cleaning Irrelevant Actions**:
  - Training set: 75%
  - Test set: 75%
  - True Positive Rate: 74%
 
![image](https://github.com/user-attachments/assets/44fce770-43b3-47ec-8077-84b6998c7aee)


### XGBoost

- **After Cleaning and Hyperparameter Tuning**:
  - Accuracy: 77%
  - True Positive Rate: 76%

- **SHAP analysis** was used to interpret the model’s results.

![image](https://github.com/user-attachments/assets/835ee4f3-4307-4bed-98fc-9f1fa6d62a49)


## Recommendations

Since only 4% of users who add items to their cart finalize the purchase, increasing the number of cart additions could potentially boost sales. Here are the key recommendations based on the analysis:

### Key Factors Influencing Cart Additions:
- Users visiting the homepage.
- Users using dropdown menus to explore products.
- Users checking delivery information on product pages.

### Targeted Actions:
- Enhance the user experience on mobile devices, as they dominate purchasing behaviors.
- Improve the visibility and usability of product exploration features, such as dropdown menus.
- Streamline the process of accessing delivery information to encourage cart additions.

### Engagement Strategies:
- Focus on returning customers, as they are more likely to complete purchases.
- Create targeted promotions or reminders to re-engage users who have previously added items to their carts.

## Conclusion

This project has successfully identified key factors and behaviors influencing cart additions and purchases. By acting on these insights, the online store can reduce cart abandonment rates and improve overall conversion rates.

