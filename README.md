# Employee Attrition Prediction Using Machine Learning

## Project Overview
This project predicts whether an employee is likely to leave an organization using a Decision Tree Classification algorithm. It uses employee-related information to train and evaluate a machine learning model.

## Objectives
- Predict employee attrition.
- Preprocess numerical and categorical data.
- Train and evaluate a Decision Tree classifier.
- Analyze important features affecting employee attrition.
- Save and reuse the trained model.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## Dataset
The project uses an HR Employee Attrition dataset containing employee demographics, job details, satisfaction levels, working experience, and attrition status.

## Machine Learning Workflow
1. Load and explore the dataset.
2. Check missing values and class distribution.
3. Separate features and target.
4. Split data into training and testing sets.
5. Encode categorical variables using OneHotEncoder.
6. Train a Decision Tree classifier.
7. Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.
8. Compare the original and balanced models.
9. Visualize feature importance.
10. Save and reload the model and encoder.
11. Predict attrition for a sample employee.

## Results

| Metric | Original Model | Balanced Model |
|---|---:|---:|
| Accuracy | 83.67% | 79.25% |
| Attrition Recall | 19% | 53% |

The balanced model improves attrition recall, helping identify more employees who may leave, while its overall accuracy is lower.

## Key Findings
- TotalWorkingYears was identified as the top feature by the balanced model's feature-importance scores.
- OverTime_Yes was identified as another important feature.
- The model's predictions are estimates and should not be used as the sole basis for employment decisions.

## Project Files
- `employee_attrition.ipynb` — Model development and evaluation.
- `employee_attrition_model.pkl` — Saved Decision Tree model.
- `employee_attrition_encoder.pkl` — Saved categorical encoder.
- `data/` — Dataset.

## How to Run
1. Install Python 3.10 or a compatible version.
2. Install the required packages:

   `pip install pandas numpy matplotlib seaborn scikit-learn joblib jupyter`

3. Open the notebook:

   `jupyter notebook employee_attrition.ipynb`

4. Run the notebook cells in order.

## Future Improvements
- Tune hyperparameters using cross-validation.
- Compare Decision Tree with Random Forest and other classifiers.
- Improve recall while monitoring precision.
- Build an interactive prediction application.

## Disclaimer
This project is intended for educational purposes. Predictions may be inaccurate and should not be used to make employment decisions about individual employees.
