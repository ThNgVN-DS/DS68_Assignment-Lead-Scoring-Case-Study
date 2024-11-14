# Lead Scoring Case Study

## Objective

An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified as leads. Moreover, the company also gets leads through past referrals.

Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X Education is around 30%. 

Although X Education generates a lot of leads, its lead conversion rate is very poor. For example, if they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should increase as the sales team will focus more on communicating with potential leads rather than making calls to everyone.

The goal is to build a logistic regression model to assign a lead score between 0 and 100 to each of the leads which can be used by the company to target potential leads. A higher score would mean that the lead is hot (most likely to convert), whereas a lower score would mean that the lead is cold (unlikely to convert). 

There are additional problems presented by the company which our model should be able to adapt to if requirements change in the future.

![Lead Conversion Process](https://cdn.upgrad.com/UpGrad/temp/189f213d-fade-4fe4-b506-865f1840a25a/XNote_201901081613670.jpg)

## Steps Followed

- **Reading Data**: Import necessary libraries and load dataset into a DataFrame.
- **Data Cleaning**: Check for missing values and handle them appropriately.
- **Exploratory Data Analysis (EDA)**: Analyze data distributions and relationships.
- **Creating Dummy Variables**: Convert categorical variables into numerical format.
- **Splitting Data**: Divide data into training and testing sets.
- **Building Model**: Develop logistic regression model using training data.
- **Making Predictions**: Use the model to predict outcomes on test data.
- **Model Evaluation**: Assess model performance using metrics such as accuracy and ROC Curve.
- **Precision-Recall Analysis**: Evaluate precision and recall rates for better insights.

## Details of Files Provided

- **Lead Score Case Study.ipynb**: The Python notebook containing code and data analysis.
- **Assignment Subjective Questions.pdf**: Document with answers to subjective questions related to the assignment.
- **Lead Score Case Study.pdf**: Final presentation summarizing findings and recommendations.
- **Leads.csv**: Dataset used for analysis containing lead information.
- **Leads Data Dictionary.xlsx**: Explanation of variables present in Leads.csv.
- **Summary.pdf**: Summary document detailing what has been accomplished throughout the project.

## Team Members

This project was collaboratively completed by:

- [Nguyen Van Thuong](https://github.com/ThNgVN-DS)
- [Uttam Kumar](https://github.com/UttamKumar2005) 
- Viswanath Padmanabhan

## Group Study Assignment

This project is part of the group study assignment for **Course 2: Machine Learning - I**, offered by **upGrad & IIITB** as part of the **Data Science Program - May 2024**.
