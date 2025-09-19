# 🚀 Spaceship Titanic 
This project tackles the **Kaggle Spaceship Titanic dataset**, a binary classification challenge where the goal is to predict whether a passenger was **Transported** to another dimension.

The notebook provides an **end-to-end machine learning pipeline**: from exploratory data analysis to feature engineering, model training, evaluation, and prediction.

## 📂 Dataset

The dataset comes from [Kaggle's Spaceship Titanic competition](https://www.kaggle.com/competitions/spaceship-titanic).
It contains information about 13,000+ passengers with features such as:

* Passenger ID, HomePlanet, Cabin, Destination
* Age, CryoSleep status, Spending details
* Target: **Transported (0 = No, 1 = Yes)**

**Note:** The raw dataset (`train.csv`, `test.csv`) is **not uploaded** to this repository due to Kaggle’s data-sharing policy.
To run this project, please download the data manually:
1. Go to the [competition page](https://www.kaggle.com/competitions/spaceship-titanic).
2. Download `train.csv` and `test.csv`.

## ⚙️ Project Pipeline

1. **Exploratory Data Analysis (EDA)**

   * Distribution plots, missing value analysis, categorical breakdowns.
2. **Feature Engineering**

   * Extracting deck, side, and group info from `Cabin` and `PassengerId`.
   * Handling missing values and encoding categorical features.
   * Scaling numerical features.
3. **Modeling**

   * Trained and compared multiple classifiers:

     * Logistic Regression
     * Random Forest
     * KNN
     * XGBoost
     * Support Vector Machine (SVM)
   * Used cross-validation for fair comparison.
4. **Evaluation**

   * Metrics: Accuracy, ROC AUC.
   * Confusion matrices and feature importance visualizations.
5. **Prediction**

   * Final model used to generate predictions on test data.


## 📊 Results

* **Best performing model:** Logistic Regression
* **Best hyperparameters:** `C=10, penalty=l2, solver=lbfgs`
* **Validation Accuracy:** 78.7%
* **Validation ROC AUC:** 0.877
