**Customer Segmentation Using K-Means Clustering**

This project performs customer segmentation using K-Means clustering based on customer transaction behavior. It helps businesses identify distinct customer groups to target them more effectively with marketing strategies.

 **Dataset Overview**

The dataset contains 5 customers with the following attributes:

| **Column**             | **Description**                             |
|---------------------|--------------------------------------------|
| `CustomerID`        | Unique customer identifier                 |
| `AnnualSpending`    | Total spending by the customer annually    |
| `PurchaseFrequency` | Number of purchases per year               |
| `AvgOrderValue`     | Average value per order                    |



 **Objective**

To segment customers into meaningful clusters based on purchasing behavior using **K-Means clustering**, and interpret the characteristics of each group to guide marketing decisions.



 **Libraries Used**

- python
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn



**Steps Performed**

1. **Data Loading & Preprocessing**
   - Loaded CSV using pandas
   - Dropped irrelevant columns (like `CustomerID`)
   - Scaled features using `StandardScaler`

2. **Elbow Method**
   - Used to determine the optimal number of clusters (WCSS plot)
   Chose k = 2

3. **K-Means Clustering**
   - Applied clustering with k=2
   - Assigned each customer a cluster label

4. **Cluster Visualization**
   - Plotted clusters using `AnnualSpending` and `PurchaseFrequency`
   - Centroids marked using black `X`

5. **Interpretation**
   - Cluster 0: High Value Customers (high frequency & high spending)
   - Cluster 1: Low Value Customers (low frequency & low spending)


**Output Sample**

Example of segmented dataset:

| CustomerID | AnnualSpending | PurchaseFrequency | AvgOrderValue | Cluster | Segment             |
|------------|----------------|-------------------|----------------|---------|---------------------|
|     1      |     1200       |        12         |      100       |    1    | Low Value Customer  |
|     2      |     3000       |        30         |      100       |    0    | High Value Customer |
|    ...     |      ...       |        ...        |      ...       |   ...   |        ...          |


**Project Structure**

customer-segmentation

├── 📄 k-means-customer-segmentation.ipynb  

├── 📄 k means data.csv

├── 📄 README.md  


**Future Enhancements**

- Use real-world datasets (e.g., from e-commerce platforms)
- Apply PCA for dimensionality reduction & better visualization
- Test with DBSCAN or Hierarchical clustering

 
If you like this project, give it a star!
