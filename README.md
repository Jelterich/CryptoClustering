# Crypto Clustering Project

## Overview
The Crypto Clustering Project analyzes cryptocurrency market data using machine learning techniques. It applies clustering algorithms and dimensionality reduction to group cryptocurrencies based on their market performance. The project also compares clustering results with and without optimization techniques such as Principal Component Analysis (PCA).

---

## Objectives
1. **Normalize Data**: Scale cryptocurrency market data to ensure comparability.
2. **Cluster Data**: Use the K-means algorithm to group cryptocurrencies.
3. **Optimize Clustering**: Apply PCA to reduce the dimensionality of the dataset and observe its effect on clustering results.
4. **Visualize Results**: Generate visualizations for elbow curves and clustered data to evaluate and compare results.

---

## File Structure
- `crypto_market_data.csv`: The dataset containing cryptocurrency market metrics.
- `Crypto_Clustering_starter_code.ipynb`: Jupyter Notebook with step-by-step code and analysis.
- `Resources/`: Folder containing additional assets and processed data.

---

## Steps and Methodology

### 1. Prepare the Data
- Import libraries (`pandas`, `hvplot.pandas`, `sklearn`).
- Load the cryptocurrency market data from `crypto_market_data.csv`.
- Normalize the data using `StandardScaler` to ensure consistency in numerical ranges.

### 2. Find the Best Value for K
- Use the **Elbow Method** to determine the optimal number of clusters for the K-means algorithm.
- Generate and visualize an elbow curve to find the inflection point, which indicates the best `k` value.

### 3. Apply K-means Clustering
- Cluster the normalized data using the K-means algorithm with the optimal `k` value.
- Assign cluster labels to each cryptocurrency.
- Visualize the clusters using scatter plots.

### 4. Optimize Clustering with PCA
- Use PCA to reduce the dataset's dimensions to three principal components.
- Analyze the explained variance to verify the effectiveness of the dimensionality reduction.
- Repeat the clustering and visualization steps on the PCA-transformed data.

### 5. Compare Results
- Compare the clustering results between the original and PCA-transformed datasets.
- Use composite plots to evaluate the impact of dimensionality reduction on clustering performance.

---

## Key Visualizations
- **Elbow Curve**: Visualizes the inertia for different `k` values to determine the optimal number of clusters.
- **Scatter Plots**: Displays clusters for original and PCA-transformed data, showing how cryptocurrencies are grouped.

---

## Questions Answered
1. **What is the optimal value for `k`?**
   - Determined from the Elbow Curve.
2. **What is the total explained variance of the three principal components?**
   - Calculated from the PCA.
3. **What is the impact of PCA on clustering results?**
   - Compared visually and analytically between original and PCA-transformed clustering results.

---

## Libraries and Tools Used
- **Python**: Main programming language.
- **Pandas**: Data manipulation and analysis.
- **HvPlot**: Interactive visualizations.
- **Scikit-learn**: Machine learning algorithms (K-means, PCA).

---

## How to Run
1. Clone the repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Open the `Crypto_Clustering_starter_code.ipynb` notebook.
4. Run the cells sequentially to complete the analysis.

---

## Future Enhancements
- Experiment with other clustering algorithms (e.g., DBSCAN, Hierarchical Clustering).
- Expand the dataset with additional cryptocurrency metrics.
- Automate the optimization process for choosing the number of clusters and PCA components.

---

## Contributors
This project was completed as part of a data analysis bootcamp. Contributions and feedback are welcome.

---

## License
This project is licensed under the MIT License - see the LICENSE file for details.

