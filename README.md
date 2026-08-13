
# 🩺 Diabetes Progression Prediction

## 📌 Project Overview

This project uses **Machine Learning** to predict diabetes disease progression based on various patient health and physiological features.

The project performs data loading, exploratory data analysis, correlation analysis, visualization, model training, prediction, and evaluation using **Linear Regression**.

> **Note:** This project predicts the `Disease_Progression` value as a continuous target. It is an academic machine-learning project and is not intended for medical diagnosis.

---

## 🎯 Objective

The main objective of this project is to:

* Analyze diabetes-related patient data.
* Identify important factors associated with disease progression.
* Build a machine learning regression model.
* Predict disease progression using patient features.
* Evaluate the performance of the trained model.

---

## 📊 Dataset

The dataset contains **442 records and 11 columns**.

### Features

| Feature               | Description                                      |
| --------------------- | ------------------------------------------------ |
| `Age`                 | Patient age                                      |
| `Sex`                 | Patient sex encoded numerically                  |
| `BMI`                 | Body Mass Index                                  |
| `Blood_Pressure`      | Blood pressure measurement                       |
| `S1_TC`               | Total cholesterol                                |
| `S2_LDL`              | Low-density lipoprotein                          |
| `S3_HDL`              | High-density lipoprotein                         |
| `S4_TCH`              | Cholesterol-related measurement                  |
| `S5_LTG`              | Triglyceride-related measurement                 |
| `S6_Glucose`          | Blood glucose measurement                        |
| `Disease_Progression` | Target variable representing disease progression |

## The notebook shows that all 11 columns are numeric and that the dataset contains **no missing values**.

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🤖 Machine Learning Model

### Linear Regression

The project uses **Linear Regression** to predict the continuous `Disease_Progression` target. The data is divided into training and testing sets using an **80/20 split** with `random_state=42`. The resulting testing set contains 89 records and 10 input features.

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Statistical Analysis
   ↓
Correlation Analysis
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Linear Regression
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Feature Importance Analysis
```

---

## 📈 Model Performance

The trained Linear Regression model achieved the following results on the test data:

| Metric   |       Score |
| -------- | ----------: |
| R² Score |  **0.4526** |
| MAE      | **42.7941** |
| RMSE     | **53.8534** |

## The notebook reports an **R² score of 0.4526**, an **MAE of 42.7941**, and an **RMSE of 53.8534**.

## ⭐ Important Features

The project also analyzes feature influence on the prediction.

The top influential features reported by the notebook include:

1. **S5_LTG**
2. **Sex**
3. **S4_TCH**
4. **BMI**

The notebook's feature-importance output shows `S5_LTG` as the strongest among the listed features.

---

## 📊 Exploratory Data Analysis

The project includes:

* Dataset preview
* Dataset shape analysis
* Column identification
* Data type analysis
* Missing-value analysis
* Descriptive statistics
* Correlation analysis
* Feature relationship visualization
* Model prediction analysis
* Feature importance visualization

The target variable `Disease_Progression` has 442 observations, with a mean of approximately **152.13** and values ranging from **25 to 346** in the dataset.

---

## 📁 Project Structure

```text
Diabetes-Progression-Prediction/
│
├── diabetes.ipynb
├── diabetes_dataset_raw.csv
├── README.md
└── images/
    ├── dataset-preview.png
    ├── correlation.png
    ├── model-performance.png
    └── feature-importance.png
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Diabetes-Progression-Prediction.git
```

### 2. Open the project

```bash
cd Diabetes-Progression-Prediction
```

### 3. Install required libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open

```text
diabetes.ipynb
```

### 6. Run all cells

Make sure the CSV dataset is available in the project folder or update the dataset path in the notebook.

---

## 🔮 Future Enhancements

The project can be improved by:

* Testing additional regression algorithms such as Random Forest, Gradient Boosting, and XGBoost.
* Performing hyperparameter tuning.
* Applying feature scaling where appropriate.
* Comparing multiple models.
* Building an interactive Streamlit dashboard.
* Adding patient-level prediction functionality.
* Deploying the trained model as a web application.
* Adding additional evaluation and visualization techniques.

---

## 👨‍💻 Author

**Sriram Sai**

B.Tech Computer Science Engineering

---

## 📜 Disclaimer

This project is developed for **educational and academic purposes only**. The predictions generated by the model should not be considered medical advice or used as a substitute for professional medical diagnosis.
