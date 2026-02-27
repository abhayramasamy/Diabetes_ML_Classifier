# Diabetes_ML_Classifier
A Machine Learning that uses Logistic Regression, Decision Tree Classifier, Voting Classifier to screen patients for the presence of diabetes.
# Diabetes Screening Classification

A machine learning project exploring classification algorithms for diabetes risk screening.

## Project Overview

This project uses health indicators (HbA1c, blood glucose, BMI, age, etc.) to predict diabetes risk. Built as a learning project to understand classification fundamentals and proper ML evaluation methodology.

## Key Results

- **Model:** Soft Voting Classifier (LogReg + Decision Tree)
- **ROC-AUC:** 97.0%
- **Accuracy:** 88.2% (vs 81% baseline HbA1c rule)
- **Improvement:** +7% over simple clinical threshold

## What I Learned

- Proper ML evaluation (stratified K-fold CV, multiple metrics)
- Precision/recall tradeoffs for screening applications
- Feature importance (HbA1c and blood glucose are primary predictors)
- Ensemble methods and when they're worth the complexity
- EDA insights (smoking is weak predictor, metabolic markers dominate)
- Importance of Simple learning algorithms when large quantities fo data is present

## Dataset

- **Source:** Muhammad Mustafa's Diabetes Prediction Dataset (Kaggle)
- **Size:** ~100,000 patient records
- **Features:** Age, Gender, BMI, HbA1c, Blood Glucose, Hypertension, Heart Disease, Smoking History

[Link to dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset)

## Tech Stack

- Python 3.x
- pandas, numpy
- scikit-learn (LogReg, DecisionTree, RandomForest, VotingClassifier)
- matplotlib, seaborn
- Jupyter Notebook

## Notebook

View the full analysis: [`diabetes_ml_note.ipynb`](./Diabetes_ML_note.ipynb)

Or run interactively on Kaggle: [https://www.kaggle.com/code/abhayramasamy/diabetes-ml-note]

## How to Run

# Clone repo
`git clone https://github.com/abhayramasamy/Diabetes_ML_Classifier/.git`

# Install dependencies
`pip install pandas numpy scikit-learn matplotlib seaborn jupyter`

# Open notebook
`jupyter notebook diabetes-classification.ipynb`


Or simply run on Kaggle (recommended - no setup needed!)

## ⚠️ Disclaimer

This is an educational project. The model is designed for learning ML concepts, not for medical diagnosis. Any health screening should be done by qualified healthcare professionals using proper diagnostic tests.

## License
GNU - PUBLIC LICENSE FEEL FREE TO USE FOR LEARNING PURPOSES!

## Credits

- Dataset: Muhammad Mustafa (Kaggle)
- Inspiration: Learning sklearn classification fundamentals
