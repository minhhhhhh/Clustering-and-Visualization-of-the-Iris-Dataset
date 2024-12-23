#Clustering and Visualization of the Iris Dataset

## Overview
This project demonstrates clustering techniques using k-means on the Iris dataset. It includes data preprocessing, clustering, and visualization to understand the distribution of different Iris species in feature space.

## Features
- **Data Preprocessing**:  
  - Standardizes features using `StandardScaler` for optimal clustering performance.
  - Separates features (`X`) and target variable (`y`) from the dataset.
  
- **Clustering with k-means**:  
  - Utilizes the k-means algorithm from `sklearn` for clustering.
  - Employs `k-means++` initialization for efficient cluster centroid placement.
  - Visualizes the clusters and centroids.

- **Visualization**:  
  - Scatter plots created with `seaborn` and `matplotlib` to illustrate the relationship between features and clusters.
  - Highlights cluster centroids for interpretability.

## Tools and Libraries
- **Pandas**: For data manipulation and loading the Iris dataset.
- **Matplotlib & Seaborn**: For creating scatter plots and visualizing clusters.
- **Scikit-learn**: For clustering (k-means), scaling, and metrics.

## Workflow
1. **Load and Explore Data**:  
   - The dataset is loaded from `data/iris.csv` and explored using `pandas`.

2. **Data Preprocessing**:  
   - Target variable (`species`) is separated for visualization purposes.
   - Features are standardized using `StandardScaler` for uniform scaling.

3. **Clustering**:  
   - k-means is applied with `k=3` clusters (corresponding to the three Iris species).
   - Clustering results (`labels_`) are stored for visualization.
   - Model parameters are examined using `km.get_params()`.

4. **Visualization**:  
   - Scatter plot showing `sepal_length` vs. `sepal_width` is created.
   - Points are styled based on actual species (`hue`) and cluster labels (`style`).
   - Cluster centroids are marked in red for clarity.

## Usage
1. Install the required libraries:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```

2. Run the script:
   ```bash
   python project5.py
   ```

3. Outputs:
   - Scatter plot showing clusters and centroids.
   - k-means model parameters displayed in the console.

## Example Visualization
- **Scatter Plot**:  
  Displays clusters with different colors and centroids marked in red.

## File Structure
- `project5.ipynb`: Jupyter Notebook containing the full implementation.
- `data/iris.csv`: Dataset containing features (`sepal_length`, `sepal_width`, `petal_length`, `petal_width`) and target variable (`species`).

