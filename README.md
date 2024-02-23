# 19_UnsupervisedLearning_Challenge
## Overview

This repository contains a main file and a correlating file with CSV files for analyzing CSV data into the Jupyter Notebook file. The directions for the module were to use knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Results

In the 19_UnsupervisedLearning_Challenge, this dataset is an analysis of different crypto market prices, which are normalized with the StandardScaler module. Further analysis was plotted using K-means model and the elbow method to select the best clustering values. A second analysis using Principal Component Analysis (PCA) was also used and modeled again with the K-means model to contrast the data to see if the model fit better by using PCA features over scaled features.

## Analysis

After carrying out principal component analysis (PCA) using three features, we found that about 88% of the variation in the dataset was explained. This means that a significant portion of the data's complexity was captured using just three dimensions. When we applied a K-means clustering model with four clusters to both the scaled (normalized) data and the data transformed by PCA, the results were highly effective. This indicates that the clustering model worked well with the reduced dimensionality, efficiently grouping the data into four distinct clusters.

<p align="center">
<img src="https://github.com/tiascott01/19_UnsupervisedLearning_Challenge/blob/main/Assets/elbows.png" width="750">
</p>

Reducing the number of features through principal component analysis (PCA) led to the formation of more cohesive clusters. This improvement likely occurred because the reduction process eliminated some of the noise or irrelevant information, thereby sharpening the focus on the patterns that matter most. Essentially, the PCA managed to distill the essence of the original normalized data into fewer principal components. This means that, despite using less information, the PCA provided a representation of the data that was both accurate and efficient, capturing the key patterns without the need for all original variables.

<p align="center">
<img src="https://github.com/tiascott01/19_UnsupervisedLearning_Challenge/blob/main/Assets/scatters.png" width="750">
</p>



## Usage

You can use this file to analyze the data in the corresponding resource CSV.

1. Open the respective file (`Crypto_Clustering.ipynb) in Jupyter Notebook.

2. Make sure that the resource and analysis directories are congruent within their respective places as listed in the script, if not change the location.

3. Run individual cells within to see the calculations.

## Resources and Citations

1. General - ChatGpt.com
