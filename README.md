# Sound Clustering Assignment

## Overview 

This project analyses and clusters unlabelled audio data using dimensionality reduction and clustering techniques. The project processes unlabelled audio files, extracts features, and visualizes clusters to evaluate performance.

The notebook performs the following tasks:

- Loads and extracts audio files from a zip file
- Extracts MFCC features using the  `librosa` library
- Applies dimensionality reduction with t-SNE(t-distributed Stochastic Neighbor Embedding) and PCA (Principal Component Analysis)
- Clusters data using K-Means and DBSCAN clustering algorithms, and evaluation of their performance
- Visualization of the results using scatter plots
- Evaluation of clustering quality using silhouette score and davies-bouldin index

## Results 

- Dimensionality reduction helped significantly in clustering by transforming the high-dimensional features into simpler 3D forms that are easier to visualize patterns and interprete the data.
- K-Means produced moderate-quality clusters, with a silhouette score of 0.4024 and Davies-Bouldin index of 1.43.
- DBSCAN failed to form meaningful clusters. This could be due to the dataset not having naturally dense regions or parameters (eps, min_samples) needing more tuning.
- Overall the K-Means performed better and was more effective for our particular dataset.

## Project Setup

1. Install dependencies
   ```
   pip install numpy matplotlib scikit-learn librosa
   ```
2. Load the data from the zip file
3. Run the notebook cells
4. Analyze results

## Conclusion

This project demonstrates how clustering algorithms can be applied to audio data. Overall, the K-Means performed better in our scenario. However, further improvements could be made by exploring more algorithms and tuning hyperparameters.
