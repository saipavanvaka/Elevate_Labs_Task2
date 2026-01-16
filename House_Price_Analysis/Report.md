Task 2: Data Cleaning Report

1. Data Cleaning Steps Taken
   Missing Value Analysis: Used .isnull().sum() to identify that columns like LotFrontage and Electrical had missing records.

Numerical Imputation: Applied Median Imputation for numerical features to ensure outliers did not skew the data.

Categorical Imputation: Applied Mode Imputation for categorical features to maintain the most frequent labels.

Feature Dropping: Removed Alley, PoolQC, Fence, and MiscFeature as they had over 80% missing data.

2. Before vs. After Comparison
   Initial Missing Values: 7,829.

Final Missing Values: 0.

Initial Features: 81.

Final Features: 77.

3. Conclusion
   The dataset is now "clean" and free of null values, making it technically ready for Machine Learning model training in the next task.
