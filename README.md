# Student Performance Analysis

## Overview

This project involves analyzing student performance data to uncover insights that can help improve academic outcomes. The dataset includes information about students' demographics, academic performance, extracurricular activities, family background, and other factors that may influence their grades.

## Dataset

The dataset provided (`Students_Grading_Dataset.csv`) contains the following key columns:

- **Demographics**: `Gender`, `Age`, `Department`
- **Academic Performance**: `Attendance (%)`, `Midterm_Score`, `Final_Score`, `Assignments_Avg`, `Quizzes_Avg`, `Participation_Score`, `Projects_Score`, `Total_Score`, `Grade`
- **Study Habits**: `Study_Hours_per_Week`, `Extracurricular_Activities`
- **External Factors**: `Internet_Access_at_Home`, `Parent_Education_Level`, `Family_Income_Level`, `Stress_Level (1-10)`, `Sleep_Hours_per_Night`

## Problem Statement

The primary objective of this analysis is to:
1. **Understand Factors Affecting Student Performance**: Identify which variables have the strongest correlation with academic success (e.g., `Total_Score` or `Grade`).
2. **Uncover Trends and Patterns**: Explore relationships between study habits, external factors, and academic outcomes.
3. **Provide Actionable Recommendations**: Derive insights that educators, policymakers, and students can use to improve academic performance.

## Exploratory Data Analysis (EDA)

### Gender Distribution

The dataset shows an almost equal distribution of males and females among the students.

### Age Distribution

The age distribution of students is relatively uniform, with most students being between 18 and 24 years old.

### Department Distribution

The dataset includes students from various departments. The distribution of students across departments is also analyzed.

## Data Cleaning

The dataset contains missing values in the following columns:
- `Attendance (%)`: 516 missing values
- `Assignments_Avg`: 517 missing values
- `Parent_Education_Level`: 1794 missing values

These missing values were handled by filling them with the median value for numerical columns and the mode for categorical columns.

## Insights and Recommendations

1. **Gender and Performance**: The analysis shows that gender does not significantly impact academic performance, as the distribution of grades is similar across genders.
2. **Age and Performance**: Older students tend to perform slightly better, possibly due to more experience and maturity.
3. **Study Habits**: Students who spend more hours studying tend to have higher grades. Encouraging better study habits could improve overall performance.
4. **External Factors**: Access to the internet at home and higher family income levels are positively correlated with better academic performance. Providing resources to students from lower-income families could help bridge this gap.

## Conclusion

This analysis provides valuable insights into the factors affecting student performance. By addressing the identified trends and patterns, educators and policymakers can implement targeted interventions to improve academic outcomes.

## Supporting Material

- Dataset: [Students Grading Dataset](https://www.kaggle.com/datasets/mahmoudelhemaly/students-grading-dataset)

## Dependencies

- pandas
- matplotlib
- seaborn

## How to Run

1. Clone the repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the Jupyter notebook `Student Performance analysis.ipynb` to see the analysis and visualizations.

```bash
git clone https://github.com/your-repo/student-performance-analysis.git
cd student-performance-analysis
pip install -r requirements.txt
jupyter notebook
