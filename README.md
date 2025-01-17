# COVID-19 Data Analysis and Modeling

This repository contains a comprehensive analysis and modeling project based on a COVID-19 dataset. The project explores various aspects of data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning modeling.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Project Workflow](#project-workflow)
4. [Analysis Highlights](#analysis-highlights)
5. [Machine Learning Models](#machine-learning-models)
6. [Dependencies](#dependencies)
7. [How to Run](#how-to-run)
8. [License](#license)

---

## Introduction

This project analyzes COVID-19 data to understand trends, relationships, and risk factors associated with the disease. The analysis involves:

- Identifying missing values and their patterns.
- Analyzing demographic distributions (e.g., age, gender).
- Investigating medical conditions and their correlation with COVID-19 risk.
- Building predictive models to classify patients based on their risk levels.

---

## Dataset
https://www.kaggle.com/datasets/meirnizri/covid19-dataset/
The dataset used in this project includes information about COVID-19 patients, such as:

- **Demographics**: Age, gender, etc.
- **Medical conditions**: Diabetes, pneumonia, hypertension, etc.
- **COVID-19 outcomes**: Classification of risk levels and death dates.

### Key Columns:
- `AGE`: Patient's age.
- `SEX`: Gender (1: Female, 2: Male).
- `CLASIFFICATION_FINAL`: Final classification of COVID-19 risk.
- `DIABETES`, `PNEUMONIA`, `HIPERTENSION`, etc.: Presence of medical conditions (1: Yes, 0: No).

---

## Project Workflow

1. **Data Loading**: Import the dataset and necessary libraries.
2. **Exploratory Data Analysis (EDA)**:
   - Visualize missing values.
   - Analyze distributions and relationships between variables.
3. **Feature Engineering**:
   - Categorize ages into groups.
   - Create derived features like `NUM_CONDITIONS` (number of medical conditions).
4. **Data Preprocessing**:
   - Handle missing values.
   - Standardize and encode features.
5. **Modeling**:
   - Train and evaluate multiple machine learning models.
6. **Evaluation**: Assess model performance using metrics such as accuracy and log loss.

---

## Analysis Highlights

### Missing Values
- Visualized using `missingno.matrix`.
- Columns with excessive missing values were removed.

### Demographic Analysis
- Age distribution: Visualized using histograms.
- Gender distribution: Analyzed using count plots.

### Medical Conditions
- Relationships between conditions (e.g., diabetes, hypertension) and COVID-19 risk were explored.

### Risk Classification
- Boxplots and count plots were used to examine the relationship between age, conditions, and risk classification.

---

## Machine Learning Models

The following models were trained and evaluated:

1. **Logistic Regression**
2. **Random Forest**
3. **XGBoost**

### Preprocessing Steps:
- Data standardization using `StandardScaler`.
- Encoding categorical variables.
- Handling outliers using winsorization.

### Evaluation Metrics:
- Accuracy
- Log Loss
- Confusion Matrix

---

## Dependencies

To run this project, install the following Python libraries:

```bash
pip install pandas numpy seaborn matplotlib missingno scikit-learn xgboost
```

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/nnichaelangello/Covid-19-Data-Analysis-and-Modeling.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Covid-19-Data-Analysis-and-Modeling
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook COVID-19 Data Analysis and Modeling.ipynb
   ```

5. Run the cells sequentially.


---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to this project by creating issues or submitting pull requests!
