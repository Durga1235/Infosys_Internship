# Heart Stroke Prediction Project

This repository contains the complete implementation and analysis for the **Heart Stroke Prediction** project. The project aims to develop a machine learning model capable of predicting the likelihood of a stroke based on patient data. 

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Milestones](#milestones)
- [Model Evaluation](#model-evaluation)
- [Results](#results)
- [Visualization](#visualization)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)

---

## Overview

The goal of this project is to:
- Build, train, and compare multiple machine learning models.
- Evaluate the performance of the best-performing model.
- Analyze dataset bias and mathematical principles behind the methods used.

This project is part of the **Heart Stroke Prediction Internship Task**. It involves multiple tasks across several milestones, from data preprocessing to model evaluation.

---

## Dataset

The dataset used in this project is `healthcare-dataset-stroke-data.csv`. It contains patient-level data including demographics, medical history, and lifestyle factors.

---

## Milestones

1. **Milestone 1**: Data Preprocessing and Cleaning
   - Addressed missing values.
   - Conducted exploratory data analysis (EDA).
   - Performed feature engineering.

2. **Milestone 2**: Initial Model Development
   - Implemented baseline models for comparison.
   - Data Visualization
   - Data Encoding

3. **Milestone 3**: Model Optimization
   - Built and compared models including Linear, Lasso, Ridge, and Logistic Regression.
   - Plotted RMSE and accuracy for performance analysis.

4. **Milestone 4**: Final Model and Project Summary
   - Combined all code into a single file.
   - Calculated Precision, Recall, F1 Score, and Accuracy for Logistic Regression.
   - Generated a Confusion Matrix graph.
   - Conducted bias analysis and mathematical concept explanation.
   - Created a PowerPoint presentation summarizing the project.

---

## Model Evaluation

The project focuses on evaluating models using metrics such as:
- Accuracy
- Precision
- Recall
- F1 Score
- Root Mean Squared Error (RMSE)

---

## Results

The Logistic Regression model achieved the best results in terms of precision and recall, making it the most suitable for this dataset. The detailed comparison of all models is included in the PowerPoint presentation.

---

## Visualization

Data visualizations, including the Confusion Matrix and key feature correlations, are part of the analysis. They provide insights into the dataset and the model's behavior.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/heart-stroke-prediction.git
2. Navigate to the project directory:
   ```bash
   cd heart-stroke-prediction
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Run the main notebook or script::
   ```bash
   jupyter notebook project.ipynb
         or
    python main.py

## Dependencies

The project requires the following libraries:
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

  Install these dependencies using:
  ```bash
  pip install -r requirements.txt

## Acknowledgments

- Dataset source: Kaggle
- Tools used: Python, Jupyter Notebook, Scikit-learn
