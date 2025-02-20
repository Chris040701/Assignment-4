# Introduction to Unsupervised Learning
Unsupervised learning is a branch of machine learning that identifies patterns and structures in data without predefined labels. This project focuses on clustering techniques to categorize sea ice and leads based on satellite data features.

## K-Means Clustering
K-Means is a fundamental unsupervised learning algorithm that partitions data into k clusters by minimizing intra-cluster variance. It assigns each data point to the nearest cluster centroid and iteratively updates centroids until convergence.
## Why Use K-Means?
- Suitable for exploratory data analysis where the structure is unknown.
- Computationally efficient and scalable to large datasets.
- Easy to interpret and implement.
## Key Steps
- Choosing K: Predefine the number of clusters.
- Centroid Initialization: Initial placement of centroids can impact results.
- Assignment Step: Each data point is assigned to its closest centroid.
- Update Step: Centroids are recomputed iteratively.
- Convergence: The algorithm stops when centroids no longer change significantly.
## Limitations
- Requires manual selection of k.
- Sensitive to initialization and outliers.

## Gaussian Mixture Models (GMM)
GMM is a probabilistic clustering method that models data as a mixture of multiple Gaussian distributions. Unlike K-Means, GMM allows for soft clustering, meaning each data point has a probability of belonging to multiple clusters.

## Why Use GMM?
- More flexible than K-Means, as it accommodates different cluster shapes.
-Provides probabilistic assignments, allowing for uncertainty estimation.
## Advantages
- Supports soft clustering.
- Captures more complex data distributions.

# Start Running
This project is developed using Google Colab, which provides free GPU/TPU access and seamless integration with Google Drive. To run this notebook, open it in Colab and execute the provided cells sequentially.

## Installation
   ```sh
pip install rasterio
pip install netCDF4
  ```
## Data Sources

- Sentinel-2 Optical Data: S2A_MSIL1C_20190301T235611_N0207_R116_T01WCU_20190302T014622.SAFE/GRANULE/L1C_T01WCU_A019275_20190301T235610/IMG_DATA/

- Sentinel-3 Altimetry Data: 
S3A_SR_2_LAN_SI_20190307T005808_20190307T012503_20230527T225016_1614_042_131______LN3_R_NT_005.SEN3
