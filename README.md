# Unsupervised Learning Reference: Discovering Wholesale Customer Segments

- Implementation of feature importance function
- Scatterplot and heatmap to check for feature correlations
- Kernel Density Estimates(KDE) to visualize feature distributions
- Feature scaling methods for when the data does not follow a normal distribution or exhibits skews
- Box-cox test
- Turkey's method outlier detection (e.g 1.5 x interquartile range)
- KDE chart of data when outliers have been removed and we have taken the log
- Conduct Principal Component Analysis(PCA)  to look at how compound features influence variance
- Dimensionality Reduction
- Map original features to principal components from "cleaned" data and PCA reduced data
- Compare K-means clustering to Gaussian Mixture models
- Silhouette scores indicate similarity between n clusters
- Apply inverse transform to new data clusters to map their centres - which represent the average customer of a given cluster
- Use model predictions to classify datapoints i.e. show which cluster they are most "similar" to
- Use supervised learning methods to classify data points - maping customer segments as target classes(labels) to input: estimated spending 

