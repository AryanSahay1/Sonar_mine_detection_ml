# Sonar_mine_detection
Machine Learning project using Logistic Regression to classify underwater sonar signals as mines or rocks using Python and Scikit-learn.

# Sonar Mine Detection Using Machine Learning

## Project Overview

This project implements a machine learning classification model to distinguish between underwater mines (metal cylinders) and rocks using sonar signal data.

The model analyzes sonar signals represented by 60 numerical features and uses Logistic Regression to classify an object as either a Mine or a Rock.

## Objectives

- Understand and explore sonar signal data.
- Perform basic exploratory data analysis (EDA).
- Train a Logistic Regression classification model.
- Evaluate model performance on training and testing datasets.
- Build a simple prediction system for new sonar observations.

## Dataset Information

**Dataset:** Connectionist Bench (Sonar, Mines vs. Rocks)

**Source:** UCI Machine Learning Repository

- Total observations: 208
- Input features: 60
- Target classes:
  - M = Mine
  - R = Rock
- Number of mine observations: 111
- Number of rock observations: 97

Dataset DOI: https://doi.org/10.24432/C5T01Q

Original research:
Gorman, R. P., & Sejnowski, T. J. (1988). Analysis of Hidden Units in a Layered Network Trained to Classify Sonar Targets. Neural Networks, 1(1), 75–89.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook
- Google Colab

## Machine Learning Workflow

1. Data collection and loading
2. Exploratory Data Analysis
3. Feature and target separation
4. Train-test splitting (90:10)
5. Logistic Regression model training
6. Model evaluation
7. Prediction on new sonar input

## Model Performance

Initial Logistic Regression results:

| Metric | Result |
|---|---:|
| Training Accuracy | 83.42% |
| Testing Accuracy | 76.19% |

The dataset was divided using stratified train-test splitting with random_state=1.

Note: These are initial results from a single train-test split. Further evaluation using cross-validation and additional classification metrics is recommended.

## Project Structure

```text
sonar-mine-detection/
├── data/
├── notebooks/
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

## Installation and Usage

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd sonar-mine-detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebook cells sequentially.

## Future Improvements

- Implement feature scaling using StandardScaler.
- Evaluate the model using a confusion matrix.
- Calculate precision, recall, F1-score and ROC-AUC.
- Apply K-Fold Cross-Validation.
- Compare Logistic Regression with SVM, KNN and Random Forest.
- Explore feature selection and hyperparameter tuning.

## Limitations

This project uses a relatively small dataset containing only 208 observations. Therefore, the reported test accuracy should not be interpreted as evidence of real-world underwater mine detection performance.

## Author

Data Science and AI/ML Master's Student

GitHub: YOUR_GITHUB_PROFILE

---

**Dataset Attribution:** Connectionist Bench (Sonar, Mines vs. Rocks), UCI Machine Learning Repository. Licensed under CC BY 4.0.
