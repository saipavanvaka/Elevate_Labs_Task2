Task 2: Data Cleaning Report (Medical Appointment Dataset)

1. Dataset Overview
   Project Name: Medical Appointment No Shows Analysis.

Goal: Clean and preprocess healthcare data to understand patient attendance patterns.

2. Data Cleaning Steps Taken
   Initial Inspection: Used .isnull().sum() to identify missing entries across all columns.

Visualizing Patterns: Generated bar charts to identify columns with the highest frequency of missing data.

Numerical Imputation: \* Filled missing values in the 'Age' column using Median Imputation.

Reasoning: The median is more robust than the mean against outliers (such as incorrect entries of 0 or 100+ years).

Categorical Imputation: \* Applied Mode Imputation for categorical features to maintain the most frequent labels.

Feature Removal: \* Dropped 'PatientId' and 'AppointmentID'.

Reasoning: These are unique identifiers that do not provide any predictive value for machine learning models.

3. Validation and Comparison
   Data Quality: Successfully reduced the total count of missing values to 0.

Dataset Size: Compared the "Before" vs. "After" shapes to ensure no rows were accidentally deleted during the cleaning process.

Export: Saved the final processed data as Cleaned_Medical_Data.csv for future modeling.
+1

4. Conclusion
   The dataset is now standardized, free of null values, and stripped of non-informative ID columns. It is ready for the next stage of the AI/ML pipeline.
