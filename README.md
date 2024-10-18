# Hospital-Readmissions

### Summary and Recommendations

#### 1. Overview

This project analyzes the Medical Information Mart for Intensive Care (MIMIC-III) clinical database, which contains health data associated for critical care admissions. Specifically, the goal is to explore patient length of stay, readmission rates within 30 days, and the most common diagnoses for patients who were readmitted within 30 days. The analysis involves key data cleaning steps, feature engineering, and exploratory data analysis (EDA) using Pandas, Matplotlib, and Seaborn.

#### 2. Data

Dataset

The MIMIC-III is a large, freely accessible database comprising deidentified health data associated with over 40,000 critical care admissions at Beth Israel Deaconess Medical Center between 2001 and 2012. MIMIC-III aims to support a wide variety of analytic studies spanning epidemiology, clinical decision-rule improvement, resource utilization, and effective treatment research.

The dataset is available from PhysioNet (https://physionet.org/content/mimiciii/1.4/) after completing required training in protecting human subjects research.

#### 3. Data Analysis Steps

1. Data Extraction and Loading
2. Data Preprocessing
3. Readmission Analysis
4. Exploratory Data Analysis (EDA)
5. Common Diagnoses for Readmitted Patients

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
