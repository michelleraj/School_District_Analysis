



# School_District_Analysis# 📚 School District Analysis

## 🔗 Project Files
- [`PyCitySchools.ipynb`](PyCitySchools-Challenge.ipynb`) – Main notebook for analysis  
- `Resources/` – Folder containing CSV data files  


---

## 📝 Overview

This project uses **Python** and **Pandas** to analyze educational data from a fictional school district. The primary objective was to extract insights from the data to assess the performance of schools based on metrics such as:

- Average test scores in reading and math  
- Overall passing percentages  
- Per-student budget analysis  
- School size and type comparisons  

The analysis was conducted by creating DataFrames from the provided CSV files and computing summary statistics and grouped metrics.

---

## 📈 Results & Observations

After modifying the dataset by replacing **9th grade scores at Thomas High School** with `NaN`, the following changes were observed:

- **District Summary:**  
  Minor changes were observed in the overall district metrics (such as average scores and passing percentages), mostly visible as slight decimal shifts.

- **School Summary:**  
  Thomas High School saw **significant improvements**, becoming the **second-best performing school** after the 9th grade data was removed.  
  - **Math and Reading passing percentages** increased by nearly **20 points**.  
  - The impact was localized to Thomas High but slightly influenced district-wide averages.

- **Analysis by School Spending and Size:**  
  - The **scores by spending per student** and **school size** remained largely consistent.
  - However, **scores by school type** reflected some change due to the reclassification impact from Thomas High School’s updated performance.

---

## ✅ Summary

By replacing the 9th-grade math and reading scores at **Thomas High School** with `NaN` values, we observed:

- A noticeable **increase in Thomas High School’s performance metrics**  
- **Improved passing percentages** for math, reading, and overall performance  
- Minor yet measurable effects on **district-wide performance statistics**  
- The update affected grouped summaries by **school type**, showing how individual schools can influence broader analysis

This project highlights the value of **data integrity** and how even small changes in the dataset can **impact analysis results** at both the micro and macro levels.

---


## [Code Link Here](PyCitySchools.ipynb)


Files:  Run PyCitySchools-Challenge.ipynb(Download Resource folder with the csv files).                     
        Run PyCitySchools.ipynb
# Overview of the School District Analysis

The purpose of the School District analysis was to use tools like python and pandas to retrieve key metrics of each school within each school districts. Created school district summary with metrics such school performance based on overall passing grade, school size and type of school. student budgets, and many more attributes by creating a data frame from the CSV file provided. 


# Results

By changing the scores of the Thomas High School the scores of the reading and math have been significantly changed, while observing the district summary only slight changes in the numbers after the decimal point are observed. At the same time, the School summary has changed significantly as the data for the school type has been changed

Replacing Thomas high school scores 9th graders have made Thomas high school be the second-best school relative to the other schools but relative to the overall analysis the percet=ntage of the scores have gone down

REplacing Thomas high school 9th graders have made an increase in the passing math and reading score to increase their score by the amount of almost 20 points

The scores by School spending remains almost the same, the score by School size also tends to remain the same but there has been some change while looking into the score by School type 

# Summary

After reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs, we can observe an increase in the scores for passing math, reading, and overall score by the amount of almost 20 points. This in turn has also brought changes to the School Summary Dataframe and District Summary data frame also taking into account the score by School types

​

