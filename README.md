# 🏥 Healthcare Analytics for Doctor Visits

A complete data analytics project exploring what drives doctor visit frequency, using the Australian Health Survey (1977–78) dataset of 5,190 individuals.

## 📌 Project Overview

Healthcare utilization is shaped by many factors — age, income, insurance coverage, chronic illness and general health — but raw survey data doesn't make these relationships obvious on its own. This project analyzes health survey data to uncover which factors actually drive doctor visits, and translates the findings into clear, evidence-based insights for healthcare planning.

## 🎯 Objective

- Understand and clean the dataset
- Explore univariate, bivariate and multivariate relationships
- Identify the strongest drivers of doctor visit frequency
- Deliver data-driven insights and recommendations

## 🗂️ Dataset

**File:** `1776250375-P2-Healthcare_Analytics_for_Doctor_Visits__1_.csv`
**Records:** 5,190 individuals

| Column | Description |
|---|---|
| `visits` | Number of doctor visits in the past 2 weeks (target variable) |
| `gender` | Male / Female |
| `age` | Age in years (scaled ÷100 in raw data) |
| `income` | Annual income (scaled, in tens of thousands) |
| `illness` | Number of illnesses in the past 2 weeks |
| `reduced` | Days of reduced activity due to illness/injury |
| `health` | General Health Questionnaire score (0–12, higher = worse) |
| `private` | Has private health insurance |
| `freepoor` | Free government insurance (low income) |
| `freerepat` | Free government insurance (elderly/disabled/veteran) |
| `nchronic` | Chronic condition, not activity-limiting |
| `lchronic` | Chronic condition, activity-limiting |

## 🛠️ Workflow

1. Data understanding (structure, types, summary statistics)
2. Data cleaning — missing values, duplicate investigation, dtype correction, outlier analysis
3. Feature engineering — readable age/income, age & income groups, consolidated insurance type, consolidated chronic status
4. Univariate analysis with storytelling for every variable
5. Bivariate analysis — doctor visits vs. every key factor
6. Multivariate analysis — correlation matrix, pivot heatmaps, pairplot
7. Key insights, recommendations and final conclusion

## 💡 Key Insights

- Doctor visits are **heavily zero-inflated** — 79.8% of respondents had zero visits in the 2-week window.
- **Reduced-activity days** is the strongest single predictor of doctor visits (correlation ≈ 0.42).
- People with a **limiting chronic condition** visit the doctor roughly **3x as often** (0.60 avg) as those with none (0.19 avg).
- Visits rise gradually with **age** and decline slightly with higher **income**.
- **Insurance type** mostly reflects *who is eligible* for it rather than independently driving extra visits.
- High-utilization patients are spread across ages and genders, not concentrated in one demographic group.

## 🧰 Technology Used

- Python 3 (Google Colab / Jupyter Notebook)
- Pandas & NumPy — data cleaning and analysis
- Matplotlib & Seaborn — data visualization
- Statistical methods — IQR outlier detection, correlation analysis
- GitHub — version control and submission

## 📁 Repository Structure
├── Healthcare_Analytics_for_Doctor_Visits_SOLUTION.ipynb # Full analysis notebook

├── 1776250375-P2-Healthcare_Analytics_for_Doctor_Visits__1_.csv # Dataset

└── README.md


## ▶️ How to Run

1. Clone the repository:
```bash
   git clone https://github.com/Mr007ok/Healthcare_Analytics_for_Doctor_Visits_SOLUTION.git
   cd Healthcare_Analytics_for_Doctor_Visits_SOLUTION
```
2. Install dependencies:
```bash
   pip install pandas numpy matplotlib seaborn
```
3. Open `Healthcare_Analytics_for_Doctor_Visits_SOLUTION.ipynb` in Jupyter Notebook or Google Colab.
4. If using Colab, upload the dataset CSV to `/content/`.
5. Run all cells in order.

## ✅ Project Status

Complete — data cleaning, feature engineering, univariate/bivariate/multivariate analysis, correlation analysis, key insights and final conclusion are all done in the notebook.

## 📜 License

This project was created for educational purposes as part of a data analytics internship project.



