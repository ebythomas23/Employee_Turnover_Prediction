

# Employee Turnover Prediction

Predicting employee turnover is crucial for organisations to plan workforce needs and understand the reasons behind employee attrition. This project aims to develop a predictive model that forecasts whether an employee will leave the organisation using machine learning techniques.

---

## Project Overview

Employee Turnover Prediction involves predicting whether an employee is likely to leave the organization. This predictive analysis helps organizations:
- Plan workforce needs by anticipating potential exits.
- Improve employee satisfaction by identifying factors influencing turnover.
- Implement targeted retention strategies to minimize turnover.

---

## Dataset

The dataset used for this project is HR.csv , which contains the following features:
- **Satisfaction Level**: Employee satisfaction score.
- **Last Evaluation**: Last performance evaluation score.
- **Number of Projects**: Number of projects completed.
- **Average Monthly Hours**: Average work hours per month.
- **Time Spent in Company**: Number of years spent in the company.
- **Work Accident**: Whether the employee had a work accident (0 or 1).
- **Promotion in Last 5 Years**: Whether the employee was promoted in the last 5 years (0 or 1).
- **Department**: Department of the employee (Sales, Technical, HR, etc.).
- **Salary**: Categorical feature with values (Low, Medium, High).
- **Left**: Target variable indicating if the employee left the company (0 = No, 1 = Yes).

---

## Project Structure

```
EMPLOYEE_TURNOVER_PREDICTION/
│
├── Dataset/
│   └── HR.csv
│
├── images/
│   ├── Logidtic_reg_confusion_matrix.png
│   ├── pipeline_logistic_reg.png
│   ├── pipeline_random_forest.png
│   ├── Random_forest_confusion_matrix.png
│   ├── ROC.png
│   └── scaled_verses_unscaled_attributes.png
│
├── notebooks/
│   └── 01_end_to_end.ipynb
│
├── venv/                  # Virtual environment files
├── .gitignore
├── README.md               # Project description and details
└── requirements.txt        # Required Python packages
```

---

## Models Used

1. **Logistic Regression**:
   - Performed moderately well but showed lower recall for class 1 (employees who left).
   - Confusion matrix showed more false negatives compared to Random Forest.

2. **Random Forest Classifier**:
   - Achieved high accuracy with balanced precision, recall, and F1-score.
   - Minimal misclassifications observed in the confusion matrix.
   - Outperformed Logistic Regression significantly.

---

## Confusion Matrix and Classification Report

We used confusion matrices and classification reports to evaluate the models, focusing on precision, recall, and F1-score.

### Random Forest
- High accuracy with balanced precision, recall, and F1-score.
- Minimal misclassifications, as shown in the confusion matrix.

### Logistic Regression
- Moderate performance but lower recall for class 1 (employees who left).
- More false negatives compared to Random Forest.

---

## ROC Curve

- The ROC curve compares model performance by plotting True Positive Rate vs. False Positive Rate.
- **Random Forest** shows a significantly higher AUC (0.98) compared to **Logistic Regression** (0.57), indicating its superior performance.

---

## Feature Importance

We analyzed feature importance to understand the factors influencing employee turnover.

### Key Findings:
- Top features influencing turnover include:
  - **Satisfaction Level** (38.80%)
  - **Average Monthly Hours** (21.03%)
  - **Last Evaluation** (19.57%)
  - **Number of Projects** (18.49%)
- Less influential features include:
  - **Time Spent in Company** (1.13%)
  - **Work Accident** (0.21%)
  - **Promotion in Last 5 Years** (0.19%)
  - **Salary** (0.20%)
  - **Sales Department (IT & R&D)** (0.18% - 0.20%)


---

## Visualisation

The following visualizations are included:
- **Confusion Matrices**:
- Logistic Regression and Random Forest
- **Pipeline Diagrams**:
- Data preprocessing and model pipelines
- **ROC Curve**:
- Comparison of True Positive Rate vs. False Positive Rate
- **Scaled vs Unscaled Attributes**:
- Visualisation of feature scaling effect

---
## How to Run

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/EMPLOYEE_TURNOVER_PREDICTION.git
    cd EMPLOYEE_TURNOVER_PREDICTION
    ```

2. **Set up Virtual Environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On MacOS/Linux
    venv\Scripts\activate     # On Windows
    ```

3. **Install Required Packages**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Notebook**:
    - Open Jupyter Notebook or VSCode and run the `01_end_to_end.ipynb` notebook.
    - This notebook performs the complete analysis, including:
      - Data Preprocessing
      - Model Training (Logistic Regression and Random Forest)
      - Model Evaluation (Confusion Matrix, Classification Report, ROC Curve)
      - Feature Importance Analysis

---

## Results

- **Random Forest Classifier** achieved 98% accuracy, outperforming Logistic Regression.
- **Satisfaction Level**, **Average Monthly Hours**, **Last Evaluation**, and **Number of Projects** were the most influential features.
- The model provides valuable insights to HR departments for developing effective employee retention strategies.

---

## Conclusion

This project demonstrates how machine learning can be leveraged to predict employee turnover and provide actionable insights for organizations. By understanding key factors influencing employee exits, companies can proactively address issues and improve employee satisfaction and retention.

---

## Author

- **Eby Thomas** - Master of Data Science student at the University of Melbourne

---
##Contact

For any queries or collaboration, feel free to reach out:
- **Email**: [ebykachappillil@gmail.com](mailto:ebykachappillil@gmail.com)
- **LinkedIn**: [Eby Thomas](https://www.linkedin.com/in/ebykachapillil/)



---
