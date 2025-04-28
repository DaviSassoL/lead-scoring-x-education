# 🧠 Lead Scoring Project – X Education

📅 **April 2025**  
👨‍💻 **Author**: Davi Sasso  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/davi-sasso-14a706232/)

---

## 🎯 Description

This is a Data Science project focused on solving a real-world business problem using supervised classification models.

The objective is to predict the probability of lead conversion based on user behavior and profile data, and to generate a **Lead Score** that allows the company to prioritize high-potential leads.

The project was developed as part of the **Data Science Experience** course during my MBA in **Data Engineering** at Mackenzie University.

---

## 📊 Dataset

- 9,240 leads
- 37 features
- Columns include lead source, website behavior, previous interactions, and whether or not the lead converted
- Binary classification: `Converted` (1) or `Not Converted` (0)

---

## 🧠 Methodology – CRISP-DM

This project followed the **CRISP-DM** methodology:

### 1. Business Understanding
X Education receives thousands of leads daily. The sales team needs to focus on leads that are more likely to convert to maximize efficiency and reduce CAC.

### 2. Data Understanding & Preparation
- Removed irrelevant or high-null columns (e.g., Tags, City)
- Replaced "Select" values with `NaN`
- Filled missing values:
  - Categorical → `'Unknown'`
  - Numerical → median
- Encoded binary values (Yes/No → 1/0)
- Dropped unique identifiers (e.g., `Lead Number`) to avoid overfitting

### 3. Modeling
- Applied supervised classification models:
  - ✅ **Logistic Regression** → AUC: 0.93 (best result)
  - Random Forest → AUC: 0.92
  - Decision Tree → AUC: 0.79
- Data split: 70% training / 30% testing

### 4. Evaluation
- ROC AUC Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)

---

## 🔢 Lead Score Generation

- Used Logistic Regression model to generate **conversion probability** for each lead
- Scaled the score from **0–1** to **0–1000** to support dashboards and CRM integration
- Final `Lead Score` helps the sales team focus on high-potential leads

---

## 📈 Results

| Scenario | Conversion Rate | Daily Sales (est.) |
|----------|------------------|--------------------|
| Current  | 30%              | 48 sales/day       |
| With Lead Scoring | up to 80% | 128 sales/day      |

🎯 **+166% sales increase potential** with the same lead processing capacity  
📉 Lower CAC, more efficiency  
📊 Smarter decision-making with a data-driven strategy

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib)
- Jupyter Notebook
- Tableau (used for visualizations during the MBA)
- PowerPoint (business presentation)
- GitHub

---

