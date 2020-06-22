# outliers_missing_values
Handle Outliers and Missing Values

* Handle Missing Data and effects of the techniques
  Different approaches to imputing missing values: 
    1. Imputation using zero, mean, median or most frequent value. Additionally, we can create a new variable that is an indicator of missingness and includes it in the model to predict the response. This is done after plugging in zero, mean, median, or most frequent value in the actual variable.

    2. Imputation using a randomly selected value

    3. Imputation with a model: The k nearest neighbor algorithm is often used to impute a missing value based on how closely it resembles the points in the training set. We choose kNN in order to capture the variability of available data. This would not be the case if we would use a linear regression model that would predict missing values along a regression line.

    4. The imputed data can be optionally standardized between 0 and 1. This might improve the performance of classification.


* Finding Outliers


  a. BoxPlot
  b. Scatter Plot
  c. z-score
  d. IQR Score
  e. Outlier Removal Clustering: Outlier Removal Clustering (ORC) is a improved version of KMean with outlier removal in each iteration. As we all know that KMean is more sensitive with outliers, and might result into local optimal centroids. For data which has lot of outliers still works well with KMean if we add outlier removal mechanism in each iteration of the KMean clustering. This will ensure the centroid calculation won't be skewed by the points far away from the cluster centroid.
