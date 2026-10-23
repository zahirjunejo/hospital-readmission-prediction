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
- Readmitted between a NO and YES, it is almost 50/50 so not much imbalance there.

### Data Dictionary

| Feature            |                                          Meaning                                          |        Type | Missing Values |
| :----------------- | :---------------------------------------------------------------------------------------: | ----------: | -------------: |
| time_in_hospital   |                      Number of days between admission and discharge                       | categorical |             no |
| num_lab_procedures |                    Number of lab tests performed during the encounter                     |         int |             no |
| num_procedures     |             Number procedures except lab tests performed during the encounter             |         int |             no |
| num_medications    |              Number of distinct generic names administered during encounter               |         int |             no |
| number_outpatient  |                Number of outpatient visits in the year preceding encounter                |         int |             no |
| number_emergency   |                Number of emergency visits in the year preceding encounter                 |         int |             no |
| number_inpatient   |                Number of inpatient visits in the year preceding encounter                 |         int |             no |
| number_diagnosis   |                         Number of diagnosis entered to the system                         |         int |             no |
| diag_1             |     The primary diagnosis (coded as first three digits of ICD9); 848 distinct values      | categorical |            yes |
| diag_2             |      Secondary diagnosis (coded as first three digits of ICD9); 923 distinct values       | categorical |            yes |
| diag_3             | Additional Secondary diagnosis (coded as first three digits of ICD9); 923 distinct values | categorical |            yes |
| medical_specialty  |                           Speciality of the admitting physician                           | categorical |            yes |
