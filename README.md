

---

# IBM HR Data Analysis Using Python and SQL

## Overview
This project analyzes and predicts employee attrition within a company by combining Python for data manipulation and machine learning with SQL for efficient data storage and querying. Using HR data imported from CSV files into a MySQL database, the analysis identifies patterns and trends that contribute to employee turnover. 

The project includes visualizations, statistical analysis, and a logistic regression model to predict the likelihood of employee attrition. These insights enable organizations to make informed decisions to improve employee retention and satisfaction.

## Dataset
The dataset used for this project is available in a CSV file: [HR Data.csv](https://github.com/aishwarya0404/IBM-HR-Data-Analysis-using-Python-and-SQL/blob/main/HR%20Data.csv). It contains employee demographic information, job roles, compensation details, and attrition status. Key attributes include:

- **Age**
- **Job Role**
- **Monthly Income**
- **Department**
- **Attrition Status** (Yes/No)
- **Years at Company**
- **Education**
- **Job Satisfaction**
- **Work-Life Balance**

## Installation
Ensure Python (version 3.7 or later) is installed. Set up the required environment using the following steps:

1. Install Python libraries:
   ```bash
   pip install pandas mysql-connector-python seaborn matplotlib scikit-learn
   ```

2. Set up a MySQL server and create a database named `ibm`.

## Usage
1. **Prepare the CSV Files**:
   - Place the HR dataset (`HR Data.csv`) in the project directory.

2. **Update the Script**:
   - Modify the Python script to reflect the file path and desired table names.

3. **Run the Script**:
   - Execute the Python script to:
     - Import data into the MySQL database.
     - Perform data analysis and visualization.
     - Train and evaluate the logistic regression model.

## Data Import
The dataset is imported into the MySQL database with the following steps:

1. **Reading CSV Files**:
   - CSV files are loaded into Pandas DataFrames.

2. **Handling Missing Values**:
   - NaN values are replaced with `None` to ensure compatibility with SQL.

3. **Table Creation**:
   - Tables are dynamically created in the database if they do not already exist, with column names adjusted to SQL naming conventions.

## Data Analysis
The analysis explores key trends, such as:

- **Average Monthly Income** by job role and department.
- **Attrition Patterns** across demographic and job-related factors.
- Identification of high-risk groups based on factors like age, job satisfaction, and years at the company.

## Data Visualization
Visualizations created using **Seaborn** and **Matplotlib** include:

- **Count Plots**: Illustrating attrition rates across different departments and job roles.
- **Histograms**: Showing distributions of numeric variables, such as monthly income and age.
- **Scatter Plots**: Exploring relationships between variables, like age and monthly income.

## Model Training
A **Logistic Regression** model is trained to predict employee attrition:

1. **Feature Preprocessing**:
   - Numeric features are standardized using `StandardScaler` for better model performance.

2. **Model Evaluation**:
   - The model is trained on a training dataset and evaluated on a test dataset using key metrics.

3. **Performance Metrics**:
   - The model's accuracy, precision, recall, and F1-score are assessed using a **confusion matrix** and **classification report**.

## Results
Key findings from the analysis and modeling include:

- **Attrition Trends**: Certain job roles and age groups exhibit higher attrition rates.
- **Monthly Income Influence**: Employees with lower monthly incomes are more likely to leave the organization.
- **Model Performance**: The logistic regression model effectively predicts employee attrition, with detailed performance metrics provided in the evaluation.

## Acknowledgments
The dataset for this project is sourced from publicly available HR data repositories. It serves as a valuable resource for exploring employee attrition patterns and developing predictive models.

---

