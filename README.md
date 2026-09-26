# World-Happiness
Regression 
# Team [Your Team Name]

**Members:** [Name 1], [Name 2], [Name 3], [Name 4]
**Track:** Predictive Modelling (Regression)
**Event:** Sherubtse Hackathon 2026 — "Bhutan by Data: Analyse. Predict. Innovate."

## Problem
We were tasked with analysing [dataset name] and building a model to predict [target variable — e.g., "a country's happiness score (Life Ladder)"] using available socioeconomic indicators. Understanding what drives this outcome can help identify actionable areas for improvement.

## Approach
1. **Exploratory Data Analysis:** Examined the distribution of the target variable, checked for missing values, and analysed relationships between features using correlation heatmaps and scatterplots.
2. **Data Cleaning:** Handled missing values using median imputation for numeric columns. Identified and removed [any leakage/redundant columns you dropped, e.g., "a derived rank feature that leaked target information"].
3. **Feature Engineering:** [Describe what you added — e.g., "Created a regional grouping feature (South Asia vs. rest of world) to enable comparative analysis."]
4. **Model Building:** Compared three regression models — Linear Regression (baseline), Random Forest, and XGBoost — using an 80/20 train-test split.
5. **Model Selection:** Selected the best-performing model based on RMSE and R² on the held-out test set, then confirmed the result using 5-fold cross-validation to ensure it wasn't a lucky split.
6. **Interpretation:** Extracted feature importance from the winning model to identify the strongest predictors.



## Results
- **Best model:** [e.g., "Random Forest"]
- **MAE:** [your value]
- **RMSE:** [your value]
- **R² Score:** [your value]
- **Cross-validated R² (mean ± std):** [your value]
- **Top predictive features:** [e.g., "Log GDP per capita, Social support, and Healthy life expectancy were the three strongest predictors."]

## Key Insight
[One or two sentences stating your actual finding — e.g., "Our analysis shows that social support and GDP per capita together explain the majority of variation in happiness scores, while generosity has minimal predictive power — suggesting that economic stability and community connection matter more than individual charitable behavior."]

## Tools & Libraries
Python, pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn

## Limitations
- [e.g., "Regional grouping used a manually defined list of countries rather than an official classification."]
- [e.g., "Given the time constraint, hyperparameter tuning was limited to the best-performing model only."]
- [Any other honest caveat — missing data handling, small sample size, etc.]

## How to Reproduce
1. Ensure the dataset file is in the same directory as the notebook/script.
2. Install dependencies: `pip install pandas numpy scikit-learn xgboost matplotlib seaborn`
3. Run all cells in `[your notebook filename].ipynb` in order (or `python [your script name].py`).
4. Outputs (charts, model comparison table) will be generated in the working directory.
