# Heart Stroke Prediction

This project aims to predict the likelihood of heart strokes based on a healthcare dataset. The dataset includes various health-related attributes, and the project involves data cleaning, analysis, and model building to provide insights into stroke prediction.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Observations](#observations)
- [Installation](#installation)


## Project Overview

Heart strokes are a leading cause of death worldwide. This project focuses on building a predictive model to identify individuals at risk of stroke based on their health metrics. By analyzing factors such as BMI, blood pressure, and age, we aim to provide valuable insights for healthcare professionals.

## Dataset

The dataset used in this project is the `healthcare-dataset-stroke-data.csv`, which contains the following features:

- **id**: Unique identifier for each patient.
- **gender**: Gender of the patient.
- **age**: Age of the patient.
- **hypertension**: Indicates if the patient has hypertension (0 = No, 1 = Yes).
- **heart_disease**: Indicates if the patient has heart disease (0 = No, 1 = Yes).
- **ever_married**: Indicates marital status (0 = No, 1 = Yes).
- **work_type**: Type of work (e.g., Private, Self-employed, etc.).
- **residence_type**: Type of residence (Urban/Rural).
- **avg_glucose_level**: Average glucose level in the blood.
- **bmi**: Body Mass Index.
- **smoking_status**: Smoking status (e.g., former smoker, never smoked, etc.).
- **stroke**: Target variable indicating whether the patient had a stroke (0 = No, 1 = Yes).

## Observations

1. The dataset contains **5100 rows** and **12 columns**.
2. The `'bmi'` column has **201 missing values**, which accounts for **3.93%** of the total data.
3. Missing values in the `'bmi'` column were filled using the **mean** to retain data consistency and accuracy.


## Installation

To run this project, you need to have Python and the following libraries installed:

```bash
pip install pandas numpy
