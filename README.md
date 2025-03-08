# Customer-Segmentation

## Overview
This project applies K-Means clustering to segment customers based on their age, annual income, and spending score. The optimal number of clusters is determined using the Elbow Method, and the final clusters are visualized in a 3D scatter plot with centroids.

## Dataset
The dataset used for this analysis is `Mall_Customers.csv`, which contains customer demographic and spending data. The key features used for clustering are:
- **Age**
- **Annual Income (k$)**
- **Spending Score (1-100)**

## Steps Involved
1. **Load the Dataset**: Read the CSV file into a Pandas DataFrame.
2. **Preprocessing**:
   - Rename columns if necessary.
   - Select relevant features (`Age`, `Annual Income`, and `Spending Score`).
3. **Finding Optimal Clusters using the Elbow Method**:
   - Fit K-Means with `k = 1 to 10`.
   - Compute Within-Cluster Sum of Squares (WCSS) for each `k`.
   - Plot the WCSS values to identify the optimal number of clusters.
4. **Applying K-Means Clustering**:
   - Use the optimal `k` value (determined from the Elbow Method).
   - Assign data points to clusters.
5. **3D Visualization**:
   - Plot clusters in a 3D scatter plot.
   - Mark cluster centroids for better interpretation.

## Dependencies
Make sure you have the following Python libraries installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Running the Code
Run the Jupyter Notebook (`.ipynb`) in a Python environment:

```bash
jupyter notebook
```

Then open the notebook and run all the cells.

## Results
- The Elbow Method helps determine the optimal number of clusters.
- Customers are grouped into meaningful segments based on spending behavior and demographics.
- A 3D scatter plot visually represents the clusters along with their centroids.

## Visualization
- **Elbow Method Plot**: Helps determine the best number of clusters.
- **3D Scatter Plot**: Shows customer segmentation based on `Age`, `Annual Income`, and `Spending Score`.

