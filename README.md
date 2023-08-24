# PRML Minor Project - YouTube Comment Classification

This project focuses on YouTube comment classification using different clustering algorithms. The goal is to identify spam comments within the dataset and improve the comment quality on videos.

## Team Members
- Renu Sankhla (B21AI028)
- Arvind Kumar Sharma (B21AI006)
- Nitish Bhardwaj (B21AI056)


## Problem Statement
The dataset contains comments from various YouTubers' videos. The primary objective is to cluster the comments, with a focus on identifying and filtering out spam comments to enhance the quality of discussions.

## Pipeline

1. Data Preprocessing
2. Data Cleaning
3. Feature Engineering
4. Model Selection
5. Prediction

### Data Preprocessing
Attributes from the dataset are explored, and the 'comment (displayed)' attribute is selected for further processing. NaN values are removed, and a smaller dataset with 10,000 samples is used for analysis.

### Data Cleaning
The NLTK library is used for text preprocessing tasks such as stopword removal and lemmatization. Lemmatization ensures the reduction of words to their essential forms.

### Feature Engineering
The comment text is converted into a feature vector using the CountVectorizer from sklearn. This step involves converting words into frequency counts, and a reduced-dimension dataset is utilized.

### Model Selection
Three clustering algorithms are selected for this problem:

1. Agglomerative Clustering
2. K-means Clustering
3. Spectral Clustering

### Prediction
Manual labelling is performed on 1000 data points for evaluating the models.

## Results

### Agglomerative Clustering
Different distance metrics are evaluated, and the clustering quality is measured using Silhouette Score, Calinski Harabasz Score, and Davies Bouldin Score. However, due to limitations in available resources, the performance is not satisfactory.

### K-means Clustering
K-means clustering is implemented, and different values for the 'thresh' hyper-parameter are explored. The algorithm aims to minimize the sum of squared distances between data points and centroids.

### Spectral Clustering
Spectral clustering with two different affinity measures (RBF and nearest neighbors) is utilized. Clustering results are evaluated using Calinski-Harabasz score, Silhouette score, and Davies-Bouldin score. The clustering algorithm with nearest neighbors as the affinity measure produced better results.


