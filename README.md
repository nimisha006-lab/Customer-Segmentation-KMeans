# Customer Segmentation using K-Means Clustering

Name: Nimisha Roy
MUID: nimisharoy@mulearn

## Project Overview

This project uses the **Mall Customers** dataset to group customers into different segments using the **K-Means Clustering** algorithm. The goal is to identify customers with similar characteristics based on their age, gender, annual income, and spending score. These customer segments can help businesses create targeted marketing strategies and improve customer satisfaction.

---

## Dataset

* **Dataset:** Mall Customers
* **File:** `Mall_Customers.xls` *(CSV file with a `.xls` extension)*
* **Number of Records:** 200 customers
* **Features:**

  * CustomerID
  * Gender
  * Age
  * Annual Income (k$)
  * Spending Score (1–100)

---

## Project Approach

To complete this project, I first loaded and explored the dataset to understand its structure and identify any missing values. I then encoded the categorical data and scaled the numerical features so that all variables contributed equally to the clustering process. Next, I used the Elbow Method to determine the optimal number of clusters and built a K-Means clustering model. After assigning each customer to a cluster, I applied Principal Component Analysis (PCA) to reduce the data to two dimensions for visualization. Finally, I analyzed the characteristics of each customer segment and provided business insights and recommendations based on the clustering results.

---

## Tools and Libraries Used

* Python
* Pandas
* Matplotlib
* Scikit-learn

  * LabelEncoder
  * StandardScaler
  * KMeans
  * PCA

---

## Project Steps

1. Loaded the dataset.
2. Explored the dataset structure.
3. Checked for missing values.
4. Encoded the Gender column.
5. Scaled the data using StandardScaler.
6. Used the Elbow Method to find the optimal number of clusters.
7. Applied the K-Means clustering algorithm.
8. Added cluster labels to the dataset.
9. Reduced the data to two dimensions using PCA.
10. Visualized the customer segments.
11. Analyzed each customer segment and provided business insights.

---

## Results

The customers were grouped into **five customer segments**:

* High Income – High Spending
* High Income – Low Spending
* Middle Income – Low Spending
* Young Moderate Income – High Spending
* Older Moderate Income – Low Spending

The PCA model explained approximately **59.9%** of the total variance, providing a useful two-dimensional visualization of the customer clusters.

---

## Business Insights

* The largest customer segment is **Young Moderate Income – High Spending**, making it an important group for promotions and new products.
* **High Income – High Spending** customers are the most valuable customers and should receive premium services and loyalty rewards.
* **High Income – Low Spending** customers have strong purchasing power but currently spend less, making them good targets for personalized marketing.
* **Middle Income – Low Spending** customers may respond well to discounts and loyalty programs.
* **Older Moderate Income – Low Spending** customers may prefer practical and value-for-money products.

---

## Project Structure

```text
Customer-Segmentation-KMeans/
│
├── Segmentation/
│   └── Mall_Customers.xls
│   |__ customer_segmentation.ipynb
| 
└── README.md

