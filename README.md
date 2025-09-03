#  Video Game Sales & Review Analysis (2004–2010)

## Overview
This repository explores the **Video Games dataset (2004–2010, collected by Dr. Joe Cox)** in two stages of analysis:
1. **Project 1 – Exploratory Data Analysis & Hypothesis Testing**
2. **Project 2 – Regression & Predictive Modeling (Expansion of Project 1)**

The dataset includes more than 1,000 video games with variables such as title, platform, year released, review scores, sales, and genre information.  
Our goal is to explore descriptive patterns, test hypotheses, and build predictive models to understand factors influencing game sales and classification.

---

##  Repository Structure
video-game-sales-analysis/
│── README.md
│── video_games.csv
│── EDA_and_Hypothesis_Testing.ipynb # Project 1
│── Regression_and_Modeling.ipynb # Project 2 (expansion)

---

##  Project Evolution

### **Project 1: Exploratory Data Analysis & Hypothesis Testing**
- **Focus:** Descriptive statistics and basic inference.
- **Key Questions:**
  - What proportion of games are Action titles?
  - Is the median review score greater than 80?
- **Methods:** Histograms, proportions, confidence intervals, hypothesis testing.
- **Findings:**
  - Action games had a notable presence.
  - The median review score was significantly higher than 80, suggesting generally favorable reviews.

---

### **Project 2: Regression & Predictive Modeling (Expansion)**
- **Focus:** Extends Project 1 by incorporating predictive modeling.
- **Key Questions:**
  - How do review scores, year released, used price, and max players affect U.S. sales?
  - Can we classify whether a game is third-person based on predictors like price, year, and platform?
- **Methods:** 
  - Multiple Linear Regression (OLS)  
  - Logistic Regression (Logit)  
  - Model diagnostics (linearity, multicollinearity, QQ-plots)  
  - Model evaluation (R², RMSE, Confusion Matrix, ROC, AUC)  
- **Findings:**
  - Review Score was positively correlated with U.S. sales, but the linear model had low explanatory power (R² ≈ 0.145).  
  - Logistic regression showed Platform had a significant effect, but model performance was weak (AUC ≈ 0.568, specificity = 0).  
  - Models highlight limitations in predictive ability given the available variables.  

---

##  Example Outputs

### Linear Regression
- **R²:** 0.145 (low explanatory power)  
- **RMSE:** ~0.97 million sales units  
- Interpretation: Sales are only weakly explained by review scores and selected features.  

### Logistic Regression
- **Pseudo R²:** 0.0117 (very low)  
- **AUC:** 0.568 (slightly better than random guessing)  
- Interpretation: Classifier predicts most games as third-person, leading to high sensitivity but poor specificity.  

---

##  Limitations
- Dataset lacks important predictors such as **genre, marketing budget, brand recognition, or developer reputation**.  
- Models showed **low predictive power**, so results should be interpreted cautiously.  

---

##  Future Work
- Include additional predictors (genre type, marketing spend, developer reputation, player reviews over time).  
- Explore **advanced machine learning models** (decision trees, random forests) for improved predictive performance.  
- Study **time trends** in game popularity across platforms to support developers in strategic planning.  

---

##  Tech Stack
- **Language:** Python (3.12)  
- **Libraries:** pandas, numpy, matplotlib, seaborn, statsmodels, scikit-learn  

---

 **Summary:**  
- **Project 1**: Focused on EDA and hypothesis testing.  
- **Project 2**: Expanded to regression and classification models, showing progression from **statistical analysis → predictive modeling**.  
Together, these projects demonstrate both **foundational statistical analysis** and **entry-level machine learning approaches** to real-world datasets.

