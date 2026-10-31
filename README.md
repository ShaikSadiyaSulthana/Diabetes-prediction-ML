# Diabetes-prediction-ML
Diabetes prediction using Machine Learning
# Machine Learning-Based Diabetes Prediction Using Clinical and Health-Related Features

## 1. Project Overview

This project focuses on using Machine Learning techniques to classify diabetes status based on clinical and health-related measurements.

The objective is to compare different machine learning algorithms and identify how effectively they classify individuals as diabetic or non-diabetic using available health data.

This project is developed as part of the **Biology for Engineers – Experiential Learning Assignment**.

## 2. Objectives

- Study the application of Artificial Intelligence and Machine Learning in healthcare.
- Analyse clinical and health-related features associated with diabetes.
- Preprocess and prepare the dataset for machine learning.
- Train and compare multiple classification algorithms.
- Evaluate model performance using different evaluation metrics.
- Understand the biological relevance of important predictive features.

## 3. Dataset

**Dataset:** Pima Indians Diabetes Dataset

**Source:** [GitHub – Pima Indians Diabetes Dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv)

Dataset information:
- Total records: 768
- Input features: 8
- Target variable: Outcome
- Classification type: Binary classification

### Features Used

| Feature | Description |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure |
| SkinThickness | Triceps skinfold thickness |
| Insulin | Serum insulin level |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Diabetes pedigree function |
| Age | Age of the individual |
| Outcome | Diabetes status (0 or 1) |

## 4. Machine Learning Algorithms

The following five classification algorithms are compared:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Support Vector Machine (SVM)
4. Random Forest
5. Gradient Boosting

## 5. Data Preprocessing

The following preprocessing techniques are used:

- Identification of invalid zero values in selected clinical measurements.
- Treatment of these values as missing data.
- Median imputation.
- Feature standardisation where required.
- Stratified training and testing split.
- Cross-validation for model selection and hyperparameter tuning.

## 6. Model Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall (Sensitivity)
- Specificity
- F1-score
- Matthews Correlation Coefficient (MCC)
- Receiver Operating Characteristic – Area Under the Curve (ROC-AUC)

Confusion matrices and ROC curves are also used to understand model performance.

## 7. Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 8. Project Structure

```text
Diabetes-Prediction-Using-Machine-Learning/
│
├── diabetes_prediction.py
├── diabetes_prediction.ipynb
├── cleaned_dataset.csv
├── README.md
│
└── results/
    ├── model_comparison.png
    ├── roc_curves.png
    ├── confusion_matrix.png
    └── feature_importance.png
```

## 9. How to Run the Project

1. Clone or download this repository.
2. Open the Jupyter Notebook in Google Colab.
3. Upload the required dataset.
4. Install the required Python libraries if they are not already available.
5. Run the notebook cells in order.
6. Review the generated evaluation metrics and visualisations.

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 10. Results

The five machine learning algorithms are compared using the evaluation metrics listed above.

The Support Vector Machine was selected based on cross-validation in the reported experiment, achieving a test ROC-AUC of 0.810 and accuracy of 70.8%.

The Random Forest achieved the highest test accuracy of 75.3% in the reported experiment.

These results are specific to the dataset and experimental setup used in this project.

## 11. Biological Significance

Glucose, BMI and the number of pregnancies were identified as influential predictors in the reported experiment.

These features have biological relevance to glucose regulation, insulin resistance and metabolic health.

The model demonstrates how machine learning can help analyse relationships between clinical measurements and diabetes status.

## 12. Limitations

- The dataset contains only 768 records.
- It represents a specific population of women aged 21 years and above.
- Some clinical measurements contain missing or invalid zero values.
- The model requires validation on larger and more diverse datasets.
- The model is intended for academic research and educational purposes, not medical diagnosis.

## 13. Disclaimer

This project is developed for educational and academic research purposes only. It is not a substitute for professional medical advice, diagnosis or treatment

## 15. Acknowledgement

We acknowledge the publicly available Pima Indians Diabetes dataset and the open-source Python libraries used in this project.

Department of Computer Science and Engineering  
Artificial Intelligence and Data Engineering  
Jain (Deemed-to-be University), Bengaluru, Karnataka, India.
