



# School_District_Analysis

## 🔗 Project Files
- #### [`Code Link Here`](PyCitySchools-Challenge.ipynb`) – Main notebook for analysis  
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


