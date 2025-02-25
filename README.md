Here’s a detailed and structured README for your Employee Turnover Prediction project. It’s humanized, concise, and covers all the essential sections needed for a professional portfolio.

---

# Employee Turnover Prediction

Predicting employee turnover is crucial for organizations to plan workforce needs and understand the reasons behind employee attrition. This project aims to develop a predictive model that forecasts whether an employee will leave the organization using machine learning techniques.

---

## Project Overview

Employee turnover is a critical issue for many organizations. It measures the total number of employees who leave an organization in a given period. Accurately predicting employee turnover enables companies to:

- Plan workforce requirements effectively.
- Identify the reasons for high attrition rates.
- Improve employee satisfaction and retention.

This project explores different machine learning models to predict employee turnover and provides insights into the factors influencing employee retention.

---

## Dataset

The dataset used for this project is `HR.csv`, which contains the following features:
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

```plaintext
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
├── venv/
│
├── .gitignore
├── README.md
└── requirements.txt
```

---

## Models Used

1. **Logistic Regression**:
   - Performed moderately well with lower recall for employees who left.
   - Confusion Matrix shows more false negatives compared to Random Forest.

2. **Random Forest Classifier**:
   - Achieved high accuracy with balanced precision, recall, and F1-score.
   - Minimal misclassifications observed in the Confusion Matrix.

---

## Performance Evaluation

### Confusion Matrix and Classification Report

- Evaluated model performance using confusion matrices and metrics like precision, recall, and F1-score.
- Random Forest outperformed Logistic Regression with higher accuracy and balanced classification metrics.

### ROC Curve

- Plotted ROC curves to compare model performance.
- Random Forest achieved a significantly higher AUC (0.98) compared to Logistic Regression (0.57).

### Feature Importance

- Examined feature importance to understand which factors impact employee turnover.



---

## Visualization

The following visualizations are included:
- **Confusion Matrices**:
  - Logistic Regression and Random Forest
- **Pipeline Diagrams**:
  - Data preprocessing and model pipelines
- **ROC Curve**:
  - Comparison of True Positive Rate vs. False Positive Rate
- **Scaled vs Unscaled Attributes**:
  - Visualization of feature scaling effect

---

## Installation and Setup

1. **Clone the repository**:
```bash
git clone https://github.com/your_username/EMPLOYEE_TURNOVER_PREDICTION.git
```

2. **Navigate to the project directory**:
```bash
cd EMPLOYEE_TURNOVER_PREDICTION
```

3. **Create and activate a virtual environment**:
```bash
python3 -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

4. **Install required libraries**:
```bash
pip install -r requirements.txt
```

5. **Run the Jupyter Notebook**:
```bash
jupyter notebook notebooks/01_end_to_end.ipynb
```

---

## Requirements

- Python 3.x
- Jupyter Notebook
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

All dependencies are listed in the `requirements.txt` file.

---

## Results and Insights

1. **Random Forest**:
   - Achieved **98% accuracy** with a balanced F1-score across classes.
   - High recall for both classes indicating robust prediction capability.

2. **Logistic Regression**:
   - Achieved **76% accuracy**, but struggled with recall for employees who left.
   - More false negatives compared to Random Forest.

3. **Feature Importance**:

    - We analyzed feature importance to understand the factors influencing employee turnover.
    - Top features influencing turnover include:
    - **Satisfaction Level** (38.80%)
    - **Average Monthly Hours** (21.03%)
    - **Last Evaluation** (19.57%)
    - **Number of Projects** (18.49%)
    - These features have the most significant impact on predicting whether an employee will leave.
    - Less influential features include:
     - **Time Spent in Company** (1.13%)
    - **Work Accident** (0.21%)
    - **Promotion in Last 5 Years** (0.19%)
    - **Salary** (0.20%)
    - **Sales Department (IT & R&D)** (0.18% - 0.20%)


---

## Conclusion

- The **Random Forest model** is the best performer with a high accuracy rate and balanced classification metrics.
- **Feature importance analysis** provides valuable insights into the factors influencing employee turnover.
- These results can help organizations:
  - Identify key drivers of employee attrition.
  - Implement targeted employee retention strategies.
  - Optimize workforce planning and resource allocation.

---

## Future Improvements

- **Hyperparameter Tuning**:
  - Further optimize model performance using GridSearchCV or RandomizedSearchCV.
- **Cross-Validation**:
  - Implement cross-validation to enhance model generalization.
- **Additional Models**:
  - Experiment with other ensemble methods like Gradient Boosting or XGBoost.
- **Deep Learning**:
  - Explore neural network architectures for enhanced predictive accuracy.

---

## Acknowledgments

- This project is inspired by the need to understand employee turnover and improve organizational retention strategies.
- Special thanks to the creators of the `HR.csv` dataset.

---

---

## Author

Developed by **Eby Thomas** - Master of Data Science Student at the University of Melbourne.

---

## Contact

For any queries or collaboration, feel free to reach out:
- **Email**: [ebykachappillil@gmail.com](mailto:ebykachappillil@gmail.com)
- **LinkedIn**: [Eby Thomas](https://www.linkedin.com/in/eby-thomas)

---
