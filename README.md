Task 2: Data Cleaning and Preprocessing
Project Overview
In this task, I performed data cleaning on two different datasets: House Prices and Medical Appointment No-Shows. My goal was to identify missing data, handle it using statistical methods, and prepare a clean version of the data for future machine learning models.

📂 Repository Structure
I have organized my work into two main folders to keep the projects separate:

House_Price_Analysis/: Contains the real estate dataset and cleaning logic.

Medical_NoShow_Analysis/: Contains the healthcare dataset and patient record cleaning.

🛠️ My Approach
1. Finding the "Gaps"
I started by using .isnull().sum() to see exactly where the data was missing. I then created bar charts to visualize these patterns, which helped me decide which columns were worth keeping.

2. Handling Missing Numbers and Categories
I didn't want to just delete rows because that loses information. Instead:

For Numbers (like Age or Lot Size): I used Median Imputation. I chose the median because it isn't affected by extreme "outlier" values, keeping the data more realistic.

For Categories (like Electrical type): I used Mode Imputation, filling the gaps with the most common answer.

3. Dropping Unnecessary Data
I made the decision to remove certain columns:

High Missing Values: In the House Prices data, features like PoolQC and Alley were over 80% empty, so I removed them to avoid confusing the model later.

Administrative IDs: In the Medical data, I removed PatientId because a random ID number doesn't help predict if someone will show up for an appointment.

✅ Final Results
After cleaning, both datasets now have 0 missing values. I have exported these as Cleaned_Dataset.csv and Cleaned_Medical_Data.csv.

🚀 How to View My Work
Open the folder for the project you want to see.

Open the .ipynb file to see my Python code and the charts I generated.

The original and cleaned CSV files are also included in each folder for comparison.# Elevate_Labs_Task2
