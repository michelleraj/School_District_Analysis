



# School_District_Analysis

## 🔗 Project Files
- #### [`Code Link Here`](PyCitySchools-Challenge.ipynb`) – Main notebook for analysis  
- `Resources/` – Folder containing CSV data files  


---

## 📝 Overview
This report provides a comprehensive analysis of student performance across the district's 15 schools, encompassing 39,170 students. The analysis evaluates key performance indicators (KPIs) including average test scores, passing rates, and the impact of school funding, size, and type on academic outcomes. The goal is to identify trends, highlight top-performing schools, and uncover areas for strategic improvement.


This project uses **Python** and **Pandas** to analyze educational data from a fictional school district. The primary objective was to extract insights from the data to assess the performance of schools based on metrics such as:

- Average test scores in reading and math  
- Overall passing percentages  
- Per-student budget analysis  
- School size and type comparisons  

The analysis was conducted by creating DataFrames from the provided CSV files and computing summary statistics and grouped metrics.

---

## 📈 Results & Observations


The district's overall performance shows a clear opportunity for improvement, particularly in mathematics.  

| **Metric**                          | **Result**     |
|-------------------------------------|----------------|
| Total Schools                       | 15             |
| Total Students                      | 39,170         |
| Total Budget                        | $82,932,330    |
| Average Math Score                  | 79.0           |
| Average Reading Score               | 81.9           |
| % Passing Math                      | 75%            |
| % Passing Reading                   | 86%            |
| % Overall Passing (Math & Reading)  | 65%            |


##  🏫 School Performance: Top & Bottom 5  

School performance varies dramatically across the district.  
The **top 5 performers** are all **Charter schools**, while the **bottom 5** are all **District schools**.  

### Top 5 Performing Schools (by % Overall Passing)  

| **School**             | **Type**   | **Overall Passing %** |
|-------------------------|------------|------------------------|
| Cabrera High School     | Charter    | 91.3%                 |
| Thomas High School      | Charter    | 90.9%                 |
| Griffin High School     | Charter    | 90.6%                 |
| Wilson High School      | Charter    | 90.6%                 |
| Pena High School        | Charter    | 90.5%                 |

---

###  Bottom 5 Performing Schools (by % Overall Passing)  

| **School**             | **Type**   | **Overall Passing %** |
|-------------------------|------------|------------------------|
| Rodriguez High School   | District   | 53.0%                 |
| Figueroa High School    | District   | 53.2%                 |
| Huang High School       | District   | 53.5%                 |
| Hernandez High School   | District   | 53.5%                 |
| Johnson High School     | District   | 53.5%                 |

---

📌 **Key Insight:**  
The type of school (**Charter vs. District**) appears to be the **strongest predictor of student success**, with a **performance gap of over 36 percentage points** in overall passing rates.  

## 💰 Performance by School Spending (Per Student)  

Analyzing performance against per-student budgeting reveals a **strong negative correlation** between spending and results.  
Schools with **lower per-student budgets** are achieving significantly higher scores.  

### 📊 Spending vs. Performance  

| **Spending Range (Per Student)** | **Average Math Score** | **Average Reading Score** | **% Overall Passing** |
|----------------------------------|-------------------------|----------------------------|------------------------|
| < $584                           | 83.5                   | 83.9                      | 90%                   |
| $585–629                         | 81.9                   | 83.2                      | 81%                   |
| $630–644                         | 78.5                   | 81.6                      | 63%                   |
| $645–675                         | 77.0                   | 81.0                      | 54%                   |

---

📌 **Key Insight:**  
The highest-performing cohort spends **< $584 per student**, while the lowest-performing cohort spends **> $645 per student**.  
This suggests that **increased budget allocation alone is not driving better academic outcomes**, and that **funds may be allocated inefficiently in higher-spending schools**. 


## 🏫 Performance by School Size  

School size has a major impact on performance.  
**Smaller and medium-sized schools dramatically outperform larger institutions.**  

### 📊 School Size vs. Performance  

| **School Size**         | **Average Math Score** | **Average Reading Score** | **% Overall Passing** |
|--------------------------|-------------------------|----------------------------|------------------------|
| Small (< 1,000)          | 83.8                   | 83.9                      | 90%                   |
| Medium (1,000–2,000)     | 83.4                   | 83.9                      | 91%                   |
| Large (2,000–5,000)      | 77.7                   | 81.3                      | 58%                   |

---

📌 **Key Insight:**  
Large schools (**2,000–5,000 students**) are struggling, with an overall passing rate **32 points lower** than small/medium schools.  
This indicates potential challenges related to **classroom size, student engagement, and resource dilution** in larger environments.  

## 🏷️ Performance by School Type  

The analysis confirms a **stark contrast in performance** between **Charter** and **District** schools.  

### 📊 School Type vs. Performance  

| **School Type** | **Average Math Score** | **Average Reading Score** | **% Overall Passing** |
|------------------|-------------------------|----------------------------|------------------------|
| Charter          | 83.5                   | 83.9                      | 90%                   |
| District         | 77.0                   | 81.0                      | 54%                   |

---

📌 **Key Insight:**  
Charter schools are exceeding District averages by a wide margin.  
The **36-point gap in overall passing rates** highlights a critical need to investigate and adopt the **effective practices, teaching methodologies, and operational structures** employed by successful Charter schools.  

## Conclusions and Recommendations
Address the District-Charter Performance Gap: Immediately initiate a deep-dive analysis into the operational, curricular, and pedagogical differences between the top Charter schools and the bottom District schools. Identify best practices that can be scaled.

Re-evaluate Budget Allocation: The inverse relationship between spending and performance is alarming. Conduct a thorough audit of fund allocation in higher-spending District schools to identify inefficiencies and reallocate resources toward proven educational strategies.

Consider School Size in Strategic Planning: The data strongly supports the benefits of smaller learning communities. Where feasible, consider initiatives to break down large schools into smaller academies or houses to create a more focused learning environment.

Focus on Mathematics: District-wide math performance is a key weakness. Implement targeted math intervention programs, particularly in the lowest-performing District schools.





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


