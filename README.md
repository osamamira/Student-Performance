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

```python
count_gender = df['Gender'].value_counts()
plt.pie(count_gender, labels=count_gender.index, autopct='%1.1f%%', startangle=90)
plt.title('Gender Distribution')
plt.show()
