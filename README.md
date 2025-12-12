# 💼 San Francisco Employee Salary Analysis (2011–2018)

## 📌 Project Overview
This project provides a detailed analysis of **312,882 salary records** of San Francisco public employees from 2011–2018.  
The study examines compensation patterns, workforce structure, pay disparities, and builds a **machine learning model** to classify employees into **Low, Medium, and High** pay categories.

The analysis includes:
- Salary distribution across years and job roles  
- Key compensation drivers (Base Pay, Overtime, Benefits)  
- Department-level spending patterns  
- Workforce trends  
- Predictive modeling with Logistic Regression, Random Forest, and XGBoost  

This project supports better **budget planning, payroll forecasting, and compensation transparency**.  

---

## 🎯 Objectives
- Analyze salary components: **Base Pay, Overtime Pay, Other Pay, Benefits**  
- Identify high-paying roles & pay anomalies  
- Study compensation trends (2011–2018)  
- Understand correlations between pay components  
- Build a model to classify employees into three compensation tiers  
- Provide insights to support public workforce management  

---

## 🛠️ Tools & Technologies
- **Python**, Pandas, NumPy  
- **Matplotlib**, Seaborn  
- **Scikit-learn**  
- **Power BI**  
- **Jupyter Notebook**  

---

## 📁 Dataset Overview
**Total records:** 312,882  
**Variables:** 9  
Includes Base Pay, Overtime Pay, Other Pay, Benefits, Total Pay, Total Pay Benefits, Job Title, and Year.  

---

## 🔍 Data Cleaning & Preprocessing (Important)
### ✔ Converted object salary columns to numeric  
Non-numeric values like `"Not Provided"` were converted to NaN.  

### ✔ Missing values treated carefully
- **Benefits:** Missing replaced with **0** (reasonable for some job types)  
- **Base Pay, Overtime Pay, Other Pay:** Missing kept as NaN (unknown, not zero)  

### ✔ Removed invalid entries
- Negative pay values deleted  
- Records with Total Pay or Total Pay Benefits = 0 removed  

---

## 📊 Exploratory Data Analysis (Accurate Insights)

### **1️⃣ Base Pay is the primary driver of total compensation**
- Mean Base Pay ≈ **$70,543**  
- Median ≈ **$68,115**  
- Values range from **$0.10 to $592,394**  

### **2️⃣ Overtime is highly skewed**
- Median = **$0** → most employees do no overtime  
- Max overtime exceeds **$309,000**  
- Heavy in Police, Fire, Transit  

### **3️⃣ Benefits are a major compensation component**
- Mean Benefits ≈ **$22,350**  
- Strong effect on Total Pay Benefits  

### **4️⃣ Total Pay & Total Pay Benefits show strong variability**
- Mean Total Pay ≈ **$79,667**  
- Mean Total Pay Benefits ≈ **$102,018**  
- Max Total Pay Benefits → **$712,802**  

---

## 💼 Job Role Insights

### **Top 10 Highest Paying Roles**  
Roles such as:
- **Chief Investment Officer**  
- **General Manager (Transit Authority)**  
- **Physician Administrator**  
- **Police & Fire Department Chiefs**  

These consistently appear as top earners due to specialized skills + heavy overtime usage.  

### **Most Common Job Titles**
- Transit Operator → **17,637 employees**  
- Special Nurse → **10,796 employees**  
- Registered Nurse → **9,165 employees**  

---

## 🏢 Department-Level Insights

### **Total Pay Contribution**
Departments contributing the most:
- **Transit**
- **Fire**
- **Police**
- **Health (Nursing)**  
Each contributes **$1.8B–$2.2B** in payroll.  

### **Highest Average Base Pay**
- **Management ($127K)**  
- **Legal ($120K)**  

### **Highest Total Pay**
- **Fire ($149K)** → driven heavily by overtime  
- Police, Engineering, Legal also high  

### **Highest Total Pay Benefits**
- Fire → **$183K**  
- Management → **$164K**  
- Police → **$144K**  

### **Largest Workforces**
- Health (Nursing)  
- Transit  

---

## 📈 Yearly Trends (2011–2018)
- Base Pay, Total Pay, and Total Pay Benefits **increase steadily**  
- **2014 shows a dip** in all components before rising sharply again  

---

## 📦 Machine Learning Model

### **Target**
Classify employees into **Low, Medium, High** pay categories using quantile-based segmentation.  

### **Models Used**
- Random Forest  
- XGBoost  
- Logistic Regression  

### **Best Model: Logistic Regression**
- Accuracy: **99.76%**  
- Perfect precision/recall for all classes  
- Most interpretable + least computational cost  

---

## 🔍 Feature Importance (Random Forest)

### **Most Important Departments**
1. Maintenance  
2. Police  
3. Management  
4. Transit  

### **Important Job Titles**
- Special Assistant 21  
- Youth Commission Advisor  
- Transit Fare Inspector  
- Dispatcher roles  

---

## 🏁 Key Takeaways
- Base Pay and Benefits are the strongest drivers of total compensation  
- Overtime is concentrated in Police, Fire, and Transit  
- Executive, legal, and medical roles dominate high-salary positions  
- Workforce grew steadily from 2011–2018  
- Logistic Regression provides the best classification performance  

---
