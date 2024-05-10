# K-Means Clustering

This repository contains Jupyter Notebook files with Python code examples for performing k-means clustering on images using the scikit-learn library. The notebooks demonstrate various aspects of k-means clustering analysis on images, including segmentation, cluster analysis, and evaluation.

## Notebooks:

### 1. `Granite_Clustering.ipynb`

#### Image Description:
The image used in this notebook is a photograph of granite, typically characterized by its intricate patterns and variations in color and texture.

#### Code Description:
- **Reading and Preprocessing Image**: The notebook reads the image `Granite.jpg` using OpenCV, converts it to RGB format, and reshapes it into a 2D array of pixels.
- **Performing K-Means Clustering**: It initializes a KMeans object with a predefined number of clusters and fits it to the pixel data.
- **Segmenting Image and Analyzing Cluster Information**: The notebook creates a segmented image by replacing each pixel's RGB values with the RGB values of the cluster centroid to which it belongs. It also calculates the number of pixels in each cluster and visualizes the cluster sizes using a pie chart.
- **Elbow Method for Optimal K**: The notebook uses the elbow method to find the optimal number of clusters by plotting the within-cluster sum of squares (WCSS) for different values of `k`.

#### Results and Insights:
- The segmented image reveals distinct clusters representing different colors and patterns present in the granite.
- The pie chart provides insights into the distribution of colors and patterns across clusters.
- The elbow method helps determine the optimal number of clusters, balancing model complexity with clustering performance.

### 2. `Lake_Clustering.ipynb`

#### Image Description:
The image used in this notebook depicts a tranquil lake surrounded by natural landscapes, characterized by various shades of blue and green.

#### Code Description:
- **Reading and Preprocessing Image**: The notebook reads the image `Lake.jpg` using OpenCV, converts it to RGB format, and reshapes it into a 2D array of pixels.
- **Performing K-Means Clustering**: It initializes a KMeans object with a predefined number of clusters and fits it to the pixel data.
- **Segmenting Image and Analyzing Cluster Information**: Similar to the previous notebook, this notebook creates a segmented image, calculates the number of pixels in each cluster, and visualizes the cluster sizes using a pie chart.
- **Silhouette Analysis**: Additionally, this notebook calculates the silhouette score for different values of `k` (number of clusters) and visualizes the silhouette plot for each value of `k`. This provides insights into the quality and separation of clusters.
- **Elbow Method for Optimal K**: Similar to the previous notebook, this notebook also uses the elbow method to find the optimal number of clusters.

#### Results and Insights:
- The segmented image reveals distinct clusters representing different regions of the lake, such as water, sky, and vegetation.
- Silhouette analysis provides a quantitative measure of clustering quality, helping to validate the choice of the number of clusters.
- The elbow method aids in selecting the optimal number of clusters, balancing model complexity with clustering performance.

## Requirements:

To run the notebooks, make sure you have the following dependencies installed:

- Python 3.x
- Jupyter Notebook
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- scikit-learn (`sklearn`)
- Pandas

## Usage:

1. Clone the repository to your local machine:

```bash
git clone https://github.com/your-username/k-means-clustering.git
```

2. Navigate to the cloned directory:

```bash
cd k-means-clustering
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```
