# Hospital-Readmissions

### Problem Statement

Unplanned hospital readmissions within 30 days signal deficiencies in post-discharge care and result in increased financial strain on healthcare systems. The project aims to predict readmission risks, enabling healthcare providers to focus on preventative care for high-risk patients.

### Solution Approach:

1. Data Cleaning and Preprocessing
- Missing Data Handling: Imputation for incomplete records.
- Feature Engineering: Extracted and encoded critical predictors such as hypertension, age, and gender.
- Scaling: Normalized numeric variables to ensure model performance.

2. Exploratory Data Analysis (EDA)
- Investigated readmission trends by demographics, length of stay, and common diagnoses.
- Visualized the impact of age, gender, and conditions on readmission rates.

3. Model Development
- Algorithms Tested: Logistic Regression and Random Forest.
- Feature Selection: Prioritized variables such as comorbidities, hypertension, and age.
- Hyperparameter Tuning: GridSearchCV to optimize Random Forest parameters.

4. Evaluation Metrics
- Prediction Accuracy: Achieved 82% accuracy.
- Other Metrics: Precision, recall, and F1-score validated model reliability.

### Key Findings:

Readmission Rate:
- Overall readmission rate: 8.33%.
- Highest among men with hypertension.

Length of Stay (LOS):
- Longer hospital stays were correlated with a reduced risk of readmission.

Age and Readmission:
- Older patients showed a slightly higher likelihood of readmission, requiring tailored post-discharge care.

Common Diagnoses:
- Top diagnoses among readmitted patients included hypertension, congestive heart failure, and urinary tract infections.

### Challenges: 

- Handling Large-Scale Data: Optimized feature extraction from extensive and partially unstructured records.

- Class Imbalance: Managed through SMOTE to ensure robust model predictions for minority classes.

### Future Directions: 

- Expand Analysis: Incorporate socio-economic factors and insurance data to understand external influences on readmission.
- Real-Time Monitoring: Develop real-time predictive systems for immediate interventions.
- Model Explainability: Use SHAP or LIME to enhance interpretability for clinical stakeholders.
- Bias Audits: Evaluate and mitigate potential biases affecting demographic groups.



#### 6. Key Findings
      
Readmission Rate:

- The code calculates the overall readmission rate within 30 days, which is displayed as a percentage. This metric provides a high-level overview of how often patients are readmitted shortly after discharge. This information is valuable for healthcare administrators to assess hospital performance and identify potential areas for improvement in patient follow-up care.

Length of Stay:

- The distribution of length of stay is visualized through a histogram. This distribution can help identify the typical length of hospital stays and detect any anomalies (e.g., unusually long or short stays).

- The boxplot comparing length of stay for readmitted and non-readmitted patients suggests whether longer stays are associated with a higher or lower likelihood of readmission.

Age vs. Readmission:

- A boxplot showing age vs. readmission within 30 days helps determine whether age plays a role in the likelihood of being readmitted. Insights from this analysis may point to whether older patients are more prone to readmission.

Gender and Readmission:

- The count plot comparing readmission rates between genders provides insights into whether gender affects the likelihood of readmission. This information can guide further exploration into gender-specific healthcare needs.

Most Common Diagnoses:

- The top 10 most common ICD-9 diagnoses among readmitted patients are displayed. Diagnoses such as hypertension (code 4019), urinary tract infection (code 5990), and congestive heart failure (code 4280) are frequently seen among readmitted patients. This insight can help focus efforts on managing these conditions more effectively to prevent readmissions.

Source: https://www.kaggle.com/datasets/asjad99/mimiciii
