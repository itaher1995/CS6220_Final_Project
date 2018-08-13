# File Directory

## Jupyter Notebooks
* FMA-DataWarngling (original FMA-Dataset) -- The file containing all data wrangling and preprocessing.
* FMA-SVMKMeans (originally FMA-Taher) -- A file that contains the work for Support Vector Machines such as the hyperparameter tuning. Also contains further data wrangling for SVM such as SMOTE and Tomeklinks and for KMeans it contains PCA.
* FMA-Unsupervised-GMM -- A file that contains the work done for Gaussian Mixture Models and extra data wrangling such as PCA
* FMA-Insights -- A file that contains the linear SVM model developed using our original design matrix without any SMOTE or Tomeklinks and the new labels from clustering

## Datasets
* fma_metadata (not on git) -- All the original metadata used to develop the model, is a data dump from the Free Music Archive (found online)
* FMADataset-cleaned -- The dataset developed from merges of the original metadata files
* FMADataset-reduced-with-pca -- The dataset developed from using pca on the transformed data
* FMDatasetTrans-cleaned -- The dataset that had the box cox transformation applied to it
* response -- The response variables (pre-labeled genres)