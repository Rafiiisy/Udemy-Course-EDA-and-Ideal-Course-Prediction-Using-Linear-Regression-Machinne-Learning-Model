# Udemy Course EDA and Ideal Course Prediction Using Linear Regression

## Project Overview
This project aims to analyze and predict ideal course characteristics on Udemy, an online learning platform. By leveraging exploratory data analysis (EDA) and a linear regression machine learning model, the project provides insights into course pricing, popularity, and characteristics, helping aspiring course creators design optimal courses.

## Why This Project?
### Problem Statement
Creating a successful online course requires understanding various factors like pricing, content duration, and student engagement. This project addresses:
- What makes an ideal Udemy course?
- How do features like price, subscribers, reviews, and content duration impact course success?

### Goal
To uncover actionable insights and relationships between course features to assist course creators in optimizing their content and pricing strategies.

---

## Dataset
### Source
The dataset used is from Kaggle: [Udemy Courses Dataset](https://www.kaggle.com/datasets/andrewmvd/udemy-courses). It comprises data from four subjects:
- Web Development
- Musical Instruments
- Graphic Design
- Business Finance

### Key Features
- `Price`
- `Number of Subscribers`
- `Number of Reviews`
- `Rating`
- `Content Duration`
- `Number of Lectures`
- `Year`
- `Subject`

---

## Data Preparation
### Steps:
1. **Data Cleaning**: Removed null and duplicate values.
2. **Encoding**: Converted non-numeric features into numerical representations.
3. **Transformation & Standardization**: Addressed skewness and outliers.
4. **Correlation Analysis**: Dropped highly correlated features to avoid multicollinearity.
5. **Data Splitting**: Divided data into training and testing sets.

---

## Exploratory Data Analysis (EDA)
### Key Insights:
- **Course Pricing**:
  - Most courses are paid, and expensive courses dominate across all subjects.
- **Subjects**:
  - Web Development leads in every category, while Musical Instruments lags behind.
- **Content Duration**:
  - Free courses tend to have shorter durations.
  - Web Development courses offer the longest average duration (~3.5 hours).
- **Subscribers & Reviews**:
  - Positive correlation exists between the number of subscribers and reviews.
  - No significant relationship between price and subscribers.
- **Trends Over Time**:
  - Udemy's peak year for course engagement was 2016.

---

## Modeling
### Target Variable:
- `Price`

### Model Performance:
- **Training Error**:
  - Mean Absolute Error (MAE): 0.69
  - Mean Absolute Percentage Error (MAPE): 1.14
- **Testing Error**:
  - MAE: 0.70
  - MAPE: 1.22

### Key Coefficients:
- `log_subscribers`: A 1-unit increase results in a 0.0082 increase in standardized price.
- `log_lectures`: A 1-unit increase results in a 0.441 increase in standardized price.
- `log_rating`: A 1-unit increase results in a 0.1196 increase in standardized price.
- `Year`: A 1-unit increase results in a 0.152 increase in standardized price.

---

## Business Recommendations
To create a successful Udemy course:
1. **Target Subject**: Web Development
2. **Price Range**: $175 - $200
3. **Course Level**: "All Levels"
4. **Content Duration**: 15-18 hours
5. **Optimize Title**: Include popular keywords to enhance discoverability

---


---

## Acknowledgments
Special thanks to Kaggle for providing the dataset and the resources that made this project possible.
