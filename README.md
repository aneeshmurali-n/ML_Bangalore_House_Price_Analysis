# ML_Bangalore_House_Price_Analysis
This project focusing on statistical analysis to understand and prepare data for potential machine learning applications. The dataset `house_price.csv` includes property prices in Bangalore. The analysis aims to perform exploratory data analysis (EDA), detect and handle outliers, check data distribution and normality, and analyze correlations.

## Dataset

- **Filename**: `house_price.csv`
- **Description**: Contains property prices in Bangalore. The main focus is on the "price per square foot" column.

## Tasks and Methodology

### Q1. Basic Exploratory Data Analysis (EDA)
- **Objective**: Perform initial analysis to understand the dataset.
- **Steps**:
  1. Load the dataset.
  2. Examine basic statistics and structure.

### Q2. Outlier Detection and Handling
- **Objective**: Identify and manage outliers using various methods.
- **Methods**:
  - **a) Mean and Standard Deviation**:
    - Compute mean and standard deviation of the "price per square foot."
    - Define outliers as values outside of mean ± (k * standard deviation), where k is typically 2 or 3.
  - **b) Percentile Method**:
    - Compute percentiles (e.g., 1st and 99th).
    - Define outliers as values below the 1st percentile or above the 99th percentile.
  - **c) IQR (Interquartile Range) Method**:
    - Calculate the IQR (Q3 - Q1).
    - Define outliers as values outside of Q1 - 1.5 * IQR and Q3 + 1.5 * IQR.
  - **d) Z Score Method**:
    - Compute Z-scores for the "price per square foot."
    - Define outliers as values with Z-scores beyond ±3.
- **Handling**: Remove or adjust outliers using trimming, capping, or imputation (mean/median).

### Q3. Box Plot Analysis
- **Objective**: Evaluate which outlier removal method is most effective.
- **Steps**:
  1. Generate box plots for the "price per square foot" column before and after outlier removal for each method.
  2. Compare the box plots to determine the best method for removing outliers.

### Q4. Distribution and Transformation
- **Objective**: Analyze the distribution of the "price per square foot" and apply transformations if necessary.
- **Steps**:
  1. Create a histplot to visualize the distribution of the "price per square foot."
  2. Apply transformations (e.g., log transformation) if the data is skewed.
  3. Compute and compare skewness and kurtosis before and after the transformation.

### Q5. Correlation Analysis and Heatmap
- **Objective**: Analyze correlations between numerical columns and visualize them.
- **Steps**:
  1. Compute the correlation matrix for all numerical columns.
  2. Plot a heatmap to visualize these correlations.

### Q6. Scatter Plot Analysis
- **Objective**: Examine relationships between pairs of numerical variables.
- **Steps**:
  1. Create scatter plots to visualize the correlation between pairs of numerical variables.

## Requirements

Ensure you have the following Python libraries installed:
- pandas
- numpy
- matplotlib
- seaborn
- scipy

Install these libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn scipy

