# Hospital Stay Duration Prediction

A machine learning project to predict a patient’s **time in hospital** using a public real-world healthcare dataset. The project focuses on regression modeling, data preprocessing, and evaluation using common regression metrics.

## Project Overview

Predicting hospital stay duration can help improve hospital resource planning, bed allocation, and patient flow management. This project uses a Linear regression approach to estimate `time_in_hospital` from structured clinical and administrative features.

The current baseline model achieved:

- **MAE:** 1.996
- **MSE:** 6.710
- **R² Score:** 0.234

These results suggest the model captures part of the pattern in the data, while also showing that hospital stay duration is a noisy real-world target influenced by many hidden factors.

## Dataset

- **Source:** UC Irvine 
- **Target variable:** `time_in_hospital`
- **Problem type:** Supervised regression
- **Link:** https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008

The dataset contains patient-related features that can be used to estimate how long a patient stays in the hospital.

## Objectives

- Clean and preprocess a real-world healthcare dataset
- Explore factors that may affect hospital stay duration
- Train a regression model to predict `time_in_hospital`
- Evaluate performance using standard regression metrics
- Understand the limitations of linear modeling on noisy medical data

## Workflow

1. Data loading and inspection
2. Missing value handling
3. Encoding categorical features
4. Feature selection / preprocessing
5. Train-test split
6. Model training using regression
7. Evaluation with MAE, MSE, and R²
8. Interpretation of results

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook

## Results

| Metric | Value |
|--------|-------|
| MAE | 1.996 |
| MSE | 6.710 |
| R² Score | 0.234 |

### Interpretation

- The model predicts hospital stay with an average absolute error of about **2 days**.
- The R² score shows that the model explains a limited but meaningful portion of the variance.
- The result is reasonable for a baseline model on a real-world healthcare problem, where many important factors may not be fully captured in the dataset.

## Project Structure

```bash
├── dataset/
├── notebooks/
├── README.md
├── models/
```

## Sample Use Cases

- Estimating patient stay duration at admission
- Supporting hospital planning and operations
- Understanding which features influence length of stay
- Comparing baseline regression models with more advanced methods

## Future Improvements

- Try nonlinear models such as Random Forest, XGBoost, or CatBoost
- Perform better feature engineering
- Handle skewed target distributions
- Analyze feature importance
- Compare multiple regression models
- Build a small dashboard or web app for predictions

## Key Learning

This project demonstrates that a model does not need a very high R² score to be valuable. Working with public real-world healthcare data helped build practical skills in preprocessing, model evaluation, and explaining results honestly.

## How to Run

1. Clone the repository
2. Install libraries
3. Open the notebook or run the training script
4. Review evaluation metrics and visualizations