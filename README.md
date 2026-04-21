# Cluster-analysis-on-Iris-dataset
I implemented K-Means clustering to group similar data points together based on feature similarities
1. Standardize the dataset 
Standardization is a critical preprocessing step to ensure that features with larger numerical ranges do not dominate the distance calculations in the K-Means algorithm. You can use the StandardScaler from scikit-learn to transform the four features (sepal length, sepal width, petal length, and petal width) so they have a mean of 0 and a standard deviation of 1. [4, 5, 6, 7, 8] 
2. Apply the Elbow Method
To find the optimal $k$, run the K-Means algorithm for a range of values (typically $k=1$ to $10$). For each $k$, calculate the Inertia or Within-Cluster Sum of Squares (WCSS), which measures the sum of squared distances from each point to its assigned cluster center. [9, 10, 11] 
The "elbow" occurs at the point where the rate of decrease in WCSS slows down significantly, which for the Iris dataset is at $k=3$. [2, 12] 
3. Apply K-Means and Visualize
Once $k=3$ is selected, fit the K-Means model to the standardized data and assign each data point to one of the three clusters. You can visualize these clusters using a 2D scatter plot of two primary features, such as Sepal Length vs. Sepal Width. [8, 13, 14, 15, 16] 
Final Result
Based on the elbow method, the optimal number of clusters for the Iris dataset is 3, which aligns with the three known species in the dataset.
