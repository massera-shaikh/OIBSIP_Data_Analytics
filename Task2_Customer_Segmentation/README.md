📘 Task 2 – Customer Segmentation using K-Means (Mall Customers)

Domain: Data Analytics
Intern: Shaikh Massera Firdous Abdul Rahim
Batch: AICTE OIB-SIP November P1

🔹 1. Objective

Is task ka aim Mall Customers dataset ka use karke customer segmentation karna tha taaki:

Buying patterns samjhe

Customer groups identify ho

Target marketing improve ho

Spending behaviour analyze ho

🔹 2. Dataset Description

Dataset columns:

CustomerID

Gender

Age

Annual Income (k$)

Spending Score (1–100)

Rows: 200 customers

🔹 3. Steps Performed
✔ Data Cleaning

Null values check

Basic statistics

Gender column encoding

✔ Feature Selection

Use only numeric features for clustering:

Age

Annual Income

Spending Score

✔ Scaling

StandardScaler applied.

✔ K-Means Clustering

Found optimal clusters using Elbow Method

Final model: 5 clusters

✔ Visualization

2D scatter plot

Heatmap

Pairplot

Cluster-wise insights

(Images saved in /images/ folder)

🔹 4. Key Insights

⭐ Cluster 1: High Income – High Spending (Best Customers)
⭐ Cluster 2: High Income – Low Spending (Needs Engagement)
⭐ Cluster 3: Low Income – High Spending (Value Shoppers)
⭐ Cluster 4: Low Income – Low Spending (Low Priority)
⭐ Cluster 5: Moderate Income – Average Spending (General Customers)

🔹 5. Conclusion

K-Means helped categorize customers based on income & spending behavior.
Businesses can personalize marketing strategies for each customer group.

🔹 6. Files Included

Notebook (Task2_Mall_Customers.ipynb)

Dataset (Mall_Customers.csv)

Images (/images/)

README.md
