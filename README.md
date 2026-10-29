# Customer Churn Prediction Using Machine Learning

## 📌 Project Overview

This project predicts whether a telecom customer is likely to leave the service (churn) using Machine Learning algorithms. It uses the Orange Telecom customer churn dataset and compares the performance of Logistic Regression and K-Nearest Neighbors (KNN).

The main objective is to identify customers who may leave the service and help telecom companies improve customer retention.

## 🎯 Objectives

- Analyze telecom customer data.
- Perform data preprocessing and feature engineering.
- Train Logistic Regression and KNN classification models.
- Evaluate model performance using different metrics.
- Compare the performance of both models.

## 📂 Dataset

The project uses the Orange Telecom customer churn dataset, divided into training and testing files:

- `churn-bigml-80.csv` — Training dataset
- `churn-bigml-20.csv` — Testing dataset

The dataset contains customer information such as account length, area code, international plan, voice mail plan, call duration, and churn status.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Machine Learning and model evaluation
- **Jupyter Notebook** — Development environment

## ⚙️ Project Workflow

1. **Data Loading:** Load the training and testing datasets.
2. **Data Exploration:** Check dataset dimensions, missing values, and churn distribution.
3. **Data Preprocessing:** Convert Yes/No values into numerical values and encode the Area code column.
4. **Feature Engineering:** Prepare the input features by encoding categorical data and removing the State column.
5. **Feature Scaling:** Apply StandardScaler to standardize the input features.
6. **Model Training:** Train Logistic Regression and KNN classifiers.
7. **Model Evaluation:** Evaluate both models using accuracy, precision, recall, F1-score, and confusion matrices.
8. **Model Comparison:** Compare the results to identify the better-performing model.

## 🤖 Machine Learning Algorithms

### 1. Logistic Regression

Logistic Regression is a supervised Machine Learning algorithm used for classification. It estimates the probability that a customer will churn or stay.

### 2. K-Nearest Neighbors (KNN)

KNN is a supervised Machine Learning algorithm that predicts a customer's class based on the classes of the nearest data points. In this project, the selected value is **K = 3**.

## 📊 Model Performance

The following results were obtained on the test dataset:

| Evaluation Metric | Logistic Regression | KNN (K = 3) |
|---|---:|---:|
| Accuracy | 85.31% | 88.76% |
| Precision | 45.95% | 72.73% |
| Recall | 17.89% | 33.68% |
| F1-score | 25.76% | 46.04% |

### Results and Observations

- KNN achieved higher accuracy than Logistic Regression.
- KNN achieved better precision, recall, and F1-score.
- KNN identified a larger proportion of customers who churned.
- Both models still missed some customers who actually churned.

Based on these test results, KNN performed better overall than Logistic Regression. However, further improvements are needed to identify more potential churners.

## 🚀 How to Run the Project

### Prerequisites

Install Python and the required libraries.

```bash
pip install pandas matplotlib seaborn scikit-learn jupyter
```

### Steps

1. Clone or download this repository.
2. Place both CSV dataset files in the appropriate project directory.
3. Open the Jupyter Notebook.
4. Run the notebook cells in order.
5. Review the model evaluation results and visualizations.

## 📁 Project Structure

```text
customer-churn-prediction-ml/
│
├── churn-bigml-80.csv
├── churn-bigml-20.csv
├── customer_churn_prediction.ipynb
└── README.md
```

*The filenames above are suggested. Adjust them to match the actual files in your repository.*

## 🔮 Future Improvements

- Improve recall to identify more customers likely to churn.
- Test additional classification algorithms.
- Perform hyperparameter tuning.
- Use cross-validation to select model parameters.
- Develop a simple web interface for customer churn prediction.

## 🏁 Conclusion

This project demonstrates how Machine Learning can be used to predict customer churn in the telecommunications industry. Logistic Regression and KNN were trained and evaluated using multiple performance metrics. KNN achieved better results on the test dataset, making it the better-performing model in this comparison.

The project provides a foundation for further improvements in churn prediction and customer retention.

---

**Project Type:** Machine Learning / Classification  
**Language:** Python  
**Domain:** Telecommunications
