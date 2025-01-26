# Customer Segmentation Project

## Project Overview

This project aims to segment customers based on their purchasing behavior and demographic information. By understanding distinct customer groups, the business can tailor marketing strategies, improve customer retention, and enhance overall profitability.

## Objectives

- Analyze customer transaction data to identify purchasing patterns.
- Implement clustering algorithms to group customers with similar behaviors.
- Evaluate the effectiveness of different clustering methods.
- Provide actionable insights and recommendations based on the segmentation.

## Data Description

The analysis utilizes two primary datasets:

1. **Customers.csv**: Contains demographic information of customers, including:
   - `CustomerID`: Unique identifier for each customer.
   - `Name`: Customer's full name.
   - `Age`: Customer's age.
   - `Gender`: Customer's gender.
   - `Region`: Geographic region of the customer.

2. **Transactions.csv**: Records of customer transactions, including:
   - `TransactionID`: Unique identifier for each transaction.
   - `CustomerID`: Identifier linking the transaction to a customer.
   - `Date`: Date of the transaction.
   - `Amount`: Monetary value of the transaction.

## Methodology

1. **Data Preprocessing**:
   - Loaded and merged the datasets on `CustomerID`.
   - Handled missing values and ensured data consistency.
   - Engineered features such as Recency, Frequency, and Monetary (RFM) metrics to quantify customer behavior.

2. **Feature Scaling**:
   - Applied logarithmic transformation to RFM features to address skewness.
   - Standardized features using `StandardScaler` to ensure uniformity for clustering.

3. **Clustering**:
   - Explored various clustering algorithms, including K-Means.
   - Determined the optimal number of clusters using the Elbow Method and Silhouette Analysis.
   - Evaluated cluster quality using metrics like the Davies-Bouldin Index.

4. **Visualization**:
   - Reduced dimensionality using Principal Component Analysis (PCA) for visualization.
   - Created scatter plots to illustrate customer segments.
   - Analyzed cluster profiles to derive meaningful insights.

## Results

- Identified distinct customer segments based on purchasing behavior.
- Provided insights into each segment's characteristics, such as average spending, transaction frequency, and recency.
- Offered recommendations for targeted marketing strategies tailored to each customer segment.

## Repository Contents

- `Customer_Segmentation.ipynb`: Jupyter Notebook containing the complete analysis, including data preprocessing, clustering, and visualizations.
- `Customers.csv`: Dataset containing customer demographic information.
- `Transactions.csv`: Dataset containing transaction records.
- `README.md`: This document providing an overview of the project.

## How to Run the Analysis

1. Clone this repository to your local machine.
2. Ensure you have Python 3.x installed along with the necessary libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, and `seaborn`.
3. Open the `Customer_Segmentation.ipynb` notebook using Jupyter Notebook or JupyterLab.
4. Execute the cells sequentially to reproduce the analysis.

## Conclusion

This project successfully segments customers into distinct groups based on their purchasing behavior. The insights derived from this segmentation can inform targeted marketing campaigns and strategic business decisions to enhance customer engagement and profitability.

## Acknowledgments

We acknowledge the contributions of the data science community and the developers of the libraries used in this project.

