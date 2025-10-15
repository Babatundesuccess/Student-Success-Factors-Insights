# Student-Success-Factors-Insights
This dataset contains information of 6,670 students and the factors that may affect their academic performance. It includes variables such as study habits, attendance, parental involvement, access to resources, internet access, school types, and gender. Academic results are measured through previous and final exam scores.
# 📊 Academic Performance Data Analysis Project

## 📘 Project Overview
This project investigates **seven key parameters** that influence students' academic performance using **Microsoft Excel** for statistical analysis and **Power BI** for visualization.  
The dataset contains **6,607 observations**, representing students’ exam scores and various learning-related factors.

The analysis applies:
- **Regression Analysis** (for continuous predictors)
- **t-Test** (for binary group comparisons)
- **ANOVA (Single Factor)** (for categorical predictors with 3 or more groups)

---

## 🧮 Statistical Parameters Analyzed
1. Hours Studied  
2. Attendance  
3. Access to Learning Resources  
4. Internet Access  
5. Teacher Quality  
6. School Type (Public vs Private)  
7. Gender  

Each parameter was analyzed against the dependent variable **Exam_Score**.

---

## ⚙️ Tools and Techniques Used
- **Microsoft Excel Data Analysis ToolPak**
  - Regression Analysis
  - t-Test: Two-Sample Assuming Unequal Variances
  - ANOVA: Single Factor
- **Power BI Desktop**
  - Data Visualization
  - Clustered Column and Line Charts
  - Correlation Dashboards
- **Pivot Tables and Descriptive Statistics** for summarization

---

## 📈 Parameter Analysis and Results

### **1. Hours Studied vs Exam Scores**
**Test Type:** Linear Regression  
**Model:** `Exam_Score = 61.46 + 0.289(Study_Hours)`  
- **R²:** 0.198  
- **t-Statistic:** 40.44  
- **p-value:** < 0.001  

**Interpretation:**  
There is a **strong positive correlation** between hours studied and academic performance. Every additional study hour leads to an estimated **0.29 increase in exam score**.  
✅ **Conclusion:** The number of hours studied has a **significant and positive effect** on academic performance.

---

### **2. Attendance vs Exam Scores**
**Test Type:** Linear Regression  
**Model:** `Exam_Score = 51.58 + 0.196(Attendance)`  
- **R²:** 0.338  
- **t-Statistic:** 58.03  
- **p-value:** < 0.001  

**Interpretation:**  
Attendance shows a **very strong positive effect** on exam scores, explaining **33.8% of score variability**.  
✅ **Conclusion:** **Consistent attendance** is one of the most critical predictors of academic success.

---

### **3. Access to Learning Resources vs Exam Scores**
**Test Type:** ANOVA (Single Factor)  
**Groups:** Low (1), Medium (2), High (3)  
- **F-statistic:** 64.39  
- **p-value:** 2.52E-41  

**Interpretation:**  
The mean scores differ significantly across access levels:
- **Low:** 66.20  
- **Medium:** 67.13  
- **High:** 68.09  

✅ **Conclusion:** Students with **greater access to resources** perform better academically. Resource availability is a **high-impact factor**.

---

### **4. Internet Access vs Exam Scores**
**Test Type:** t-Test (Two-Sample Assuming Unequal Variances)  
- **Mean (Access):** 67.29  
- **Mean (No Access):** 66.54  
- **t-statistic:** 3.97  
- **p-value (two-tail):** 8.14E-05  

**Interpretation:**  
Students with internet access significantly outperform those without.  
✅ **Conclusion:** **Internet availability** has a **highly significant positive impact** on academic achievement.

---

### **5. Teacher Quality vs Exam Scores**
**Test Type:** ANOVA (Single Factor)  
**Groups:** Low (1), Medium (2), High (3)  
- **F-statistic:** 17.42  
- **p-value:** 2.91E-08  

**Interpretation:**  
Performance increases with teacher quality, indicating that **teacher effectiveness directly contributes to better student outcomes**.  
✅ **Conclusion:** **Teacher quality** significantly enhances academic performance.

---

### **6. School Type (Public vs Private)**
**Test Type:** Linear Regression  
**Model:** `Exam_Score = 63.61 + 1.79(School_Type)`  
- **R²:** 0.219  
- **p-value:** 0.067  

**Interpretation:**  
Public school students performed slightly better (by about 1.79 points) than private school students, though the difference is **not statistically significant**.  
⚠️ **Conclusion:** **School type** has a **low-to-moderate impact**, suggesting other factors play a larger role.

---

### **7. Gender vs Exam Scores**
**Test Type:** Linear Regression  
**Model:** `Exam_Score = 67.29 - 0.075(Gender)`  
- **R²:** 0.000078  
- **p-value:** 0.472  

**Interpretation:**  
The effect of gender on exam scores is statistically insignificant. Both male and female students achieved similar results.  
❌ **Conclusion:** **Gender** has **no measurable impact** on academic performance.

---

## 📊 Comparative Summary

| **Parameter**          | **Test Type** | **Effect on Scores** | **p-value** | **Impact Level** |
|------------------------|---------------|----------------------|--------------|------------------|
| Hours Studied          | Regression    | Positive             | < 0.001      | **High**         |
| Attendance             | Regression    | Positive             | < 0.001      | **Very High**    |
| Access to Resources    | ANOVA         | Positive             | 2.5E-41      | **High**         |
| Internet Access         | t-Test        | Positive             | 8.1E-05      | **High**         |
| Teacher Quality         | ANOVA         | Positive             | 2.9E-08      | **Moderate–High**|
| School Type             | Regression    | Slightly Positive    | 0.067        | **Low–Moderate** |
| Gender                  | Regression    | Neutral              | 0.472        | **Negligible**   |

---

## 🧠 Key Insights
- **Attendance and study hours** are the most powerful predictors of academic success.
- **Access to educational resources and internet** greatly enhance student performance.
- **Teacher quality** significantly influences outcomes, emphasizing the importance of teacher training.
- **School type and gender** have minimal to no significant effects on exam results.

---

## 🎨 Visualization Summary (Power BI)
The dataset was visualized in Power BI using:
- **Clustered Column Charts** (for comparing groups)
- **Line Charts** (for showing trends over attendance and study hours)
- **Bar Charts** (for access categories)

Color Scheme:
- Blue gradient for academic performance metrics  
- Green tones for positive effects (e.g., attendance, study hours)  
- Neutral gray for non-significant variables  

---

## 🧾 Conclusion
The study demonstrates that academic performance is **multi-dimensional**, primarily driven by **behavioral (attendance, study hours)** and **resource-based (internet and material access)** factors.  
Efforts to improve **attendance policies**, **digital access**, and **teacher effectiveness** can substantially improve student outcomes.

---

## 🏁 Final Note
All analyses were performed using **Microsoft Excel’s Data Analysis ToolPak**.  
Results were validated using pivot tables and Power BI dashboards for accurate interpretation and visual storytelling.
