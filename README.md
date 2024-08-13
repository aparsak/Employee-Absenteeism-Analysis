# 📊 Employee Absenteeism Analysis

This project analyzes the reasons behind employee absenteeism using data collected from 2015 to 2018. The main goal is to identify patterns and correlations that might help distinguish between genuine and fake absenteeism, with the ultimate aim of minimizing work absenteeism through better hiring processes and strategies.

## Project Overview

- **Language**: Python 🐍
- **Tools**: Jupyter Notebook 📒, Pandas 🐼, NumPy 🔢, Matplotlib 📈, Seaborn 🌊
- **Dataset**: Contains records of employee absences, including reasons, dates, and other related features.

## 📁 Dataset Description

The dataset contains several features, including:
- **Absence_Reason**: The reason for the absence, coded based on ICD (International Classification of Diseases).
- **Date**: The date of absence.
- **Employee_ID**: Unique identifier for each employee.
- **Education_Level, Disciplinary_Incident, Social_Drinker_Status, Social_Smoker_Status**: Categorical features stored as numeric or boolean values.
- **Distance_to_Work**: Distance from the employee's residence to their workplace.
- **Transportation_Expense**: The cost of transportation for the employee.
  
There are more features available in the dataset. You can explore them further in the existing dataset.

## 🔍 Analysis Steps

1. **Data Preprocessing**:
    - Checked for and handled missing values.
    - Removed duplicate records.
    - Converted and extracted date-related features (month, year, weekday).
    - Converted categorical features to more descriptive labels.
    
2. **Exploratory Data Analysis (EDA)**:
    - Identified the top three most frequent reasons for absence using bar plots.
    - Created a new binary feature `Disease` to check if the reason for absence falls within a specific ICD range.
    - Analyzed the impact of social drinking and smoking on absenteeism.
    - Examined the relationship between absenteeism and distance to work, as well as transportation expenses using joint plots.

3. **🔎 Insights**:
    - Absenteeism due to specific reasons such as medical consultations or physiotherapy was prevalent.
    - Alcohol consumption showed a noticeable impact on absenteeism, particularly linked to certain reasons like dental consultations.
    - The violin plot analysis suggested that frequent alcohol consumers tend to have longer absenteeism hours.
    - Joint plots indicated some correlation between distance to work, transportation costs, and absenteeism, though further analysis using transformation techniques (e.g., Yeo-Johnson) was necessary for clearer insights.

## 🚀 How to Run

To run this project, you'll need to have Python installed along with the necessary libraries:

```bash
pip install pandas numpy matplotlib seaborn scipy
```

Load the dataset into a Jupyter Notebook and execute the code cells sequentially. The data preprocessing steps will prepare the dataset, and the subsequent analysis cells will generate visualizations and insights.

### 🔮 Future Work
- Explore more advanced machine learning models to predict absenteeism.
- Conduct deeper analysis on the impact of other categorical variables.
- Implement further data transformation and feature engineering techniques.

This project was part of the Data Mining Course at Amirkabir University of Technology.

Coded by Parsa Khadem and Sarvin Baghi.

