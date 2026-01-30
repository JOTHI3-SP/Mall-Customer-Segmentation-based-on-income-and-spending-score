# Mall-Customer-Segmentation-based-on-income-and-spending-score

# Mall Customer Segmentation Using K-Means Clustering

## Project Description
This project applies **K-Means clustering** to segment mall customers based on their **annual income and spending behavior**. The objective is to discover meaningful customer groups using **unsupervised learning** and visualize distinct purchasing patterns.

## Dataset Used
Mall customer dataset containing the following attributes:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

For clustering, the notebook specifically uses:
- **Annual Income**
- **Spending Score**

## Data Processing
- Dataset loaded and inspected for structure
- Relevant numerical features selected
- Data converted into a NumPy array for clustering
- No label encoding or target variable used (unsupervised setup)

## Model Selection (Elbow Method)
- The **Elbow Method** is used to determine the optimal number of clusters
- **WCSS (Within-Cluster Sum of Squares)** is computed for cluster counts from **1 to 10**
- The elbow curve is plotted to observe diminishing returns

### Optimal Number of Clusters
- Based on the elbow plot, the optimal number of clusters is chosen as:
  
**k = 5**

## Clustering Model
- Algorithm: **K-Means**
- Number of clusters: **5**
- Initialization and fitting performed using Scikit-learn
- Each customer is assigned a cluster label

## Visualization & Results
- Customers are visualized using a **2D scatter plot**
- X-axis: Annual Income  
- Y-axis: Spending Score  
- Each cluster is shown in a different color
- Cluster centroids are plotted and clearly marked

### Observations from Clusters
- Distinct customer groups with similar spending behavior are formed
- High-income–high-spending and low-income–low-spending groups are clearly separated
- Cluster visualization confirms effective segmentation

## Libraries & Tools
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## How to Execute
1. Clone the repository
2. Install dependencies:
   pip install pandas numpy matplotlib scikit-learn
3. Open the notebook
4. Run cells sequentially to reproduce results

## Key Takeaway
This notebook demonstrates how **K-Means clustering combined with the Elbow Method** can be effectively used to segment customers based on purchasing patterns, providing clear visual and analytical insights without labeled data.
