# 📱 Daily Screen Time and Calorie Intake Analysis

## 📘 Project Overview
This project aims to analyze whether **daily screen time** has a measurable impact on **total calorie intake**.  
The objective is to determine if people tend to consume more calories on days when they spend more time on their phones.  
The dataset will be self-collected daily and analyzed using Python to identify any significant correlation between the two variables.

---

## 🎯 Project Motivation
In today's digital world, people spend several hours on their smartphones every day.  
This prolonged screen usage may be associated with increased calorie consumption due to habits like distracted eating, reduced physical activity, or irregular meal timing.  
The goal of this project is to examine if there is a clear relationship between **screen time** and **caloric intake**, and to quantify its strength through data analysis.

---

## 🧪 Hypothesis
- **H₁:** Daily screen time is positively correlated with total calorie intake.  
- **H₀:** There is no significant relationship between daily screen time and total calorie intake.

---

## 📊 Data Sources
- **Screen Time:** Collected from the built-in *Digital Wellbeing (Android)* or *Screen Time (iOS)* application.  
- **Calorie Intake:** Logged manually using *MyFitnessPal* or an equivalent nutrition tracking tool.  

All data will be **self-recorded** and **anonymized**.  
No external APIs or restricted data sources (e.g., Spotify, step counter) will be used.

---

## ⚙️ Data Collection and Processing
| Variable | Description | Unit |
|-----------|-------------|------|
| Date | Observation date | YYYY-MM-DD |
| Screen_Time | Total phone usage time per day | Minutes |
| Total_Calories | Total daily calorie intake | kcal |



### **Data Processing Steps**
1. Convert the `Date` column to datetime format.  
2. Ensure numeric values for `Screen_Time` and `Total_Calories`.  
3. Handle missing or inconsistent data.  
4. Remove unrealistic values (e.g., screen time > 1000 min, calories < 1000 kcal).  
5. Compute derived metric:  
   - `Calorie_Deficit = 2300 - Total_Calories`

---

## 🔍 Data Analysis & Techniques
1. **Exploratory Data Analysis (EDA):**  
   - Summary statistics (mean, median, standard deviation)  
   - Distribution plots for both variables  

2. **Correlation Analysis:**  
   - Use Pearson correlation to test the linear relationship between screen time and total calories.  

3. **Regression Modeling:**  
   - Apply a simple linear regression model:  
     ```
     Total_Calories = β₀ + β₁(Screen_Time) + ε
     ```
   - Visualize regression line and residuals.  

---

## 🎯 Expected Findings
- A positive correlation between **screen time** and **total calorie intake**.  
- Quantitative measurement of how much calorie intake increases per extra hour of screen time.  
- Insights into how technology habits may influence eating behavior.

---

## ⚠️ Limitations and Future Work
- Self-reported calorie data may contain small inaccuracies.  
- Short observation period (6–8 weeks) limits generalization.  
- Future studies could include additional variables such as sleep duration or exercise time.

---

## 💻 Technical Requirements
- **Programming Language** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`  
- **Environment:** Jupyter Notebook or VS Code  
- **Version Control:** GitHub  

---

## 📚 Sources
- Digital Wellbeing / Screen Time (Android)  
- MyFitnessPal  
- Python documentation (pandas, scikit-learn)  

---

## ✅ Summary
This project will explore the connection between **daily screen time** and **calorie intake** using self-collected real-world data.  
Through data analysis and regression modeling, it aims to determine whether higher screen exposure is linked to increased calorie consumption.

