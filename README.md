# Unsupervised Learning Reference: Discovering Wholesale Customer Segments

- Implementation of feature importance function
- Scatterplot and heatmap to check for feature correlations
- Kernel Density Estimates(KDE) to visualize feature distributions
- Feature scaling methods for when the data does not follow a normal distribution or exhibits skews
- Box-cox test
- Turkey's method outlier detection (e.g 1.5 x interquartile range)
- KDE chart of data when outliers have been removed and we have taken the log
- Conduct Principal Component Analysis(PCA)  to see how compound features influence variance
- Dimensionality Reduction
- Map original features to principal components from "cleaned" data and PCA reduced data
- Compare K-means clustering to Gaussian Mixture models
- Silhouette scores indicate similarity between n clusters
- Apply inverse transform to new data clusters to map their centres - which represent the average customer of a given cluster
- Use model predictions to classify datapoints i.e. show which cluster they are most "similar" to
- Use supervised learning methods to classify data points - maping customer segments as target classes(labels) to input: estimated spending 

# Content: Unsupervised Learning
## Project: Creating Customer Segments

### Install

This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 3.x installer and not the Python 2.7 installer. 

### Code

The notebook code is provided in the `customer_segments.ipynb` notebook file. 

### Run

In a terminal or command window, navigate to the top-level project directory `customer_segments/` (that contains this README) and run one of the following commands:

```bash
jupyter notebook customer_segments.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

## Data

The customer segments data is included as a selection of 440 data points collected on data found from clients of a wholesale distributor in Lisbon, Portugal. More information can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers).


**Features**
1) `Fresh`: annual spending on fresh products (Continuous); 
2) `Milk`: annual spending on milk products (Continuous); 
3) `Grocery`: annual spending on grocery products (Continuous); 
4) `Frozen`: annual spending on frozen products (Continuous);
5) `Detergents_Paper`: annual spending on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisnon - 1, Oporto - 2, or Other - 3} (Nominal) 

