# Lead Scoring Case Study

## Objective

An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. The company markets its courses on several websites and search engines like Google. Once these individuals arrive at the website, they might browse the courses, fill out a form for the course, or watch some videos. When they provide their email address or phone number by filling out a form, they are classified as leads. Additionally, the company also acquires leads through past referrals.

Once these leads are gathered, employees from the sales team begin making calls and writing emails. Through this process, some leads convert while most do not. The typical lead conversion rate at X Education is around 30%. 

Although X Education generates a substantial number of leads, its lead conversion rate is relatively low. For instance, if they acquire 100 leads in a day, only about 30 of them convert. To enhance this process, the company aims to identify the most promising leads, referred to as ‘Hot Leads’. By successfully identifying this group of leads, the conversion rate should improve as the sales team can focus their efforts on engaging potential leads rather than contacting every lead indiscriminately.

The goal is to build a logistic regression model that assigns a lead score between 0 and 100 to each lead. A higher score indicates that the lead is hot (most likely to convert), while a lower score suggests that the lead is cold (unlikely to convert). 

The model should also be adaptable to additional challenges presented by the company in the future.

## Steps Followed

The project involved several key stages:

- **Data Acquisition and Preparation**: 
  - The initial dataset contained 9,240 records and 37 features.
  - Categorical features were identified for conversion into dummy variables.
  - Irrelevant and incomplete data were removed, resulting in a final dataset retaining 68.97% of the original rows and increasing the conversion rate from 38.54% to 48.09%.

- **Exploratory Data Analysis (EDA)**: 
  - Visualizations using Matplotlib and Seaborn revealed critical insights, such as the influence of lead source and website engagement on conversion likelihood.

- **Feature Engineering**: 
  - Categorical features were converted into dummy variables to optimize model performance, resulting in a total of 74 features.

- **Preparing Data for Modeling**: 
  - The dataset was split into training (70%) and testing (30%) subsets.
  - Robust scaling was applied to mitigate the impact of potential outliers in numerical variables.

- **Model Building**: 
  - Recursive Feature Elimination (RFE) and stepwise elimination based on Variance Inflation Factor (VIF) and p-values were utilized to select the most relevant features.
  - The final model included 12 features at the fourth step.

- **Initial Model Evaluation**: 
  - A conventional cutoff of 0.5 was used for classification.
  - The model achieved an accuracy of 78.05% on the training set but exhibited a high number of false negatives.
  - ROC curve analysis and Precision-Recall Tradeoff analysis were conducted to optimize the classification threshold.

- **ROC Curve Optimization**: 
  - ROC curve analysis yielded an optimized cutoff of 0.418, achieving higher recall on both training and testing sets.
  - This cutoff prioritizes minimizing false negatives, aligning with X Education's goal of capturing potential leads.

- **Precision-Recall Tradeoff Optimization**: 
  - This analysis resulted in an optimized cutoff of 0.431, providing a balanced tradeoff between precision and recall.
  - This cutoff is particularly suitable for marketing campaigns where balancing between identifying potential customers and minimizing wasted resources is crucial.

## Key Learnings

This project provided valuable insights into the data science workflow:

- **EDA**: The importance of thorough EDA in identifying trends and informing feature selection.
  
- **Data Integrity**: The necessity of effectively handling missing values to maintain data integrity.
  
- **Feature Engineering**: The role of feature engineering in enhancing model performance.
  
- **Evaluation Metrics**: Understanding how different evaluation metrics can guide business decisions regarding lead prioritization.
  
- **Optimized Cutoffs**: How to determine and select appropriate optimized cutoffs based on varying business objectives.

## Conclusion

This case study reinforced technical skills in data analysis and modeling while highlighting the importance of aligning analytical outcomes with business objectives. The logistic regression model, with optimized cutoffs determined through ROC curve and Precision-Recall Tradeoff analysis, provides X Education with a robust tool for predicting lead conversion. The choice of cutoff will depend on specific business objectives—whether prioritizing lead capture or balancing precision and recall. Continuous monitoring of model performance is crucial to ensure alignment with evolving business needs.

## Contributors

This case study was initially intended to be a collaborative effort among three team members. However, due to communication challenges with one member and lack of participation from another, I undertook all aspects of this project independently. 

The project was completed by:

- [Nguyen Van Thuong](https://github.com/ThNgVN-DS)

## Group Study Assignment

This project is part of the group study assignment for **Course 2: Machine Learning - I**, offered by **upGrad & IIITB** as part of the **Data Science Program - May 2024**.
