# 🎮 Video Game Review Analysis (2004–2010)

## 📌 Overview  
This project analyzes a dataset of video games released between 2004 and 2010.  
The goal is to explore game genres and review scores, and to perform statistical analysis including descriptive analytics, confidence intervals, and hypothesis testing.  

---

## 📊 Dataset  
- **Source**: Dataset collected by Dr. Joe Cox (Video Games 2004–2010)  
- **Size**: ~1,770 rows, 10+ features  
- **Key Features**:  
  - `Title`: Game name  
  - `Console`: Platform (e.g., Nintendo DS, PlayStation 3)  
  - `YearReleased`: Year of release  
  - `US Sales`: Sales in millions  
  - `Review Score`: Critic review score (0–100)  
  - Genre indicators (e.g., Action, Sports)  

---

## 🧹 Methods & Workflow  

### 1. Dataset Introduction  
- **Population**: All video games released worldwide between 2004–2010  
- **Sample**: Dataset of 1,770 games  

### 2. Research Questions  
1. What percentage of video games released 2004–2010 are Action games?  
2. Is the **median review score** greater than 80?  

### 3. Data Cleaning  
- Checked for missing values → none detected  
- Standardized variable names  

### 4. Descriptive Analytics  
- Sample size: 1,770  
- Review Score summary:  
  - Mean = 68.4  
  - Median = 70  
  - Std Dev ≈ 13.9  
  - Range = 12–98  

### 5. Visualization  
![Histogram of Review Scores](results/review_score_distribution.png)  
- Distribution is slightly left-skewed  
- Most games cluster between 60–80  
- Outliers exist at both low and high extremes  

### 6. Statistical Analysis  
- **Confidence Interval**: Proportion of Action games estimated between ~58.5% and ~63.1% (95% CI)  
- **Hypothesis Test**:  
  - H₀: Median = 80  
  - H₁: Median > 80  
  - Result: Fail to reject H₀ (p ≈ 0.18), meaning there is insufficient evidence to claim median > 80  

---

## 📈 Results & Insights  
- About **61%** of video games released 2004–2010 were Action games.  
- The **median review score** is ~70, significantly below 80.  
- Distribution of scores suggests that while some games achieve very high ratings, most cluster in the average range.  
- Action genre dominates the dataset, but high review scores are not guaranteed by genre alone.  

---

## 🛠 Tools  
- Python (pandas, numpy, scipy)  
- Jupyter Notebook  
- matplotlib, seaborn  
- Statistical resampling & hypothesis testing  

---

## 🚀 How to Run  
1. Clone this repository:  
   ```bash
   git clone https://github.com/YourUsername/video-game-analysis.git
