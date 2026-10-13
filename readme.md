## Hospital Readmission Prediction

Data Source: [Link](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)

_Can patient and hospital encounter data be used to predict whether a diabetic patient will be readmitted to the hospital within 30 days?_

## Data Exploration

### Initial Findings

- About 101766 patients
- 50 columns
- Numerical variables: time in hospital, num lab procedures, num procedures, num_medications, number_outpatient, number_emergency, number_inpatient, number_diagnosis,
- Categorical variable: race, gender, age, weight, admission type id, medical specialty, diag_1, diag_2, diag_3, change, insulin, diabetesMed, readmitted
- Missing values: max_glu_serum and A1Cresult columns have some missing values. Weight may also be null value.
- Readmitted between a NO and YES, it is almots 50/50 so not much imbalance there.

### Data Dictionary

| Feature      |    Meaning     |          Type | Missing Values |
| :----------- | :------------: | ------------: | -------------: |
| Left-aligned | Center-aligned | Right-aligned |     dsdfsdfsdf |
| Row 2, Col 1 |  Row 2, Col 2  |  Row 2, Col 3 |     sfdsfsdfsf |
