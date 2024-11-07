# Heart Stroke Prediction Project

This project aims to analyze and prepare a dataset related to heart stroke prediction. The project includes two main tasks:
1. Data Visualization
2. Data Encoding

## Dataset

The dataset used in this project is titled `healthcare-dataset-stroke-data.csv`. It contains information on patient demographics, health conditions, and lifestyle choices, which are valuable in predicting heart stroke risk.

---

## Task I: Data Visualization

Data visualization helps in understanding the distribution and relationship between different features. The following steps were taken to explore the data visually using both Matplotlib and Seaborn libraries.

### Steps

1. **Framing Questions**: Relevant questions to guide our visual analysis include:
   - What is the distribution of age in the dataset?
   - How does BMI vary between males and females?
   - Is there a relationship between age and average glucose level?
   - How does heart stroke risk differ between urban and rural residents?
   - What is the distribution of work type among stroke cases?

2. **Plotting Graphs**: A variety of graphs were plotted, including histograms, bar plots, scatter plots, and a pairplot. These visualizations provide insights into the dataset's characteristics and the relationships among variables.

3. **Observations**: Each plot is followed by a brief interpretation based on the visual data.

---

## Task 2: Data Encoding

### Objective

Convert specific categorical variables to binary format (0s and 1s) using efficient methods, including `lambda` functions, to ensure the dataset is in a model-ready state.

### Steps

1. **Encoding `Residence_type`**: 
   - Convert the `Residence_type` column to binary, where 0 represents "Rural" and 1 represents "Urban".
   - **Observation**: Successfully converted `Residence_type` to binary format, where 0 = Rural and 1 = Urban.

2. **Encoding `work_type`**:
   - Created binary columns for the categories in `work_type`, specifically `Never_worked`, `Private`, and `Self_employed`.

   - **Observation**: Each `work_type` category was correctly encoded as separate binary columns, allowing the model to distinguish between different types of work without multicollinearity.

3. **Encoding `smoking_status`**:
   - Created binary columns for `smoking_status` categories, specifically `Never_smoked`, `Formerly_smoked`, and `Smokes`.
   - **Observation**: The `smoking_status` variable was successfully split into binary columns, improving model interpretability by distinguishing non-smokers, former smokers, and current smokers.

4. **Dropping Original Categorical Columns**:
   - After encoding, the original `Residence_type`, `work_type`, and `smoking_status` columns were dropped to avoid redundancy.
   - **Code**:
     ```python
     df_model = df.drop(['Residence_type', 'work_type', 'smoking_status'], axis=1)
     ```
   - **Observation**: The categorical columns have been removed, leaving only the encoded binary columns, which is optimal for model processing.



