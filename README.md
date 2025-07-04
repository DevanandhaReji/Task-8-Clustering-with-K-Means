# Task-8-Clustering-with-K-Means
Task 8: Clustering with K-Means
The dataset contains the following columns:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

For this task, we selected only:
- `Annual Income (k$)`
- `Spending Score (1-100)`

---

## Tools and Libraries

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

##  Steps Performed

### 🔹 1. Importing Libraries
Imported necessary libraries like `pandas`, `matplotlib`, `sklearn`, etc.

### 🔹 2. Loading the Dataset
Loaded the dataset using `pandas` and displayed the first few records to understand the structure.

### 🔹 3. Preprocessing the Data
Selected two relevant features:
- Annual Income (k$)
- Spending Score (1-100)

These features are best suited for clustering customers by financial behavior.

### 🔹 4. Finding Optimal Clusters - Elbow Method
Used the Elbow Method to find the best number of clusters (K) by plotting the **inertia** values against different K values.

📉 From the plot, the "elbow point" appeared at **K = 5**, which we used for clustering.

### 🔹 5. Applying K-Means Clustering
Fitted the **KMeans model** with `n_clusters=5` and predicted cluster labels for each customer. A new column `Cluster` was added to the dataset.

### 🔹 6. Visualizing the Clusters
Used **Seaborn scatterplot** to visualize the 5 clusters in 2D, based on income and spending score. Each cluster was color-coded for better understanding.

### 🔹 7. Evaluation using Silhouette Score
Calculated the **Silhouette Score**, which tells how well each point fits within its cluster.  
 **Silhouette Score: 0.554** (a good indication of defined clusters)

### 🔹 8. (Optional) PCA-based Visualization
Applied **Principal Component Analysis (PCA)** to reduce features to 2D and plotted the clusters using the transformed coordinates.
