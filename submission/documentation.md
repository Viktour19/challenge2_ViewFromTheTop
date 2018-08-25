
**Documentation**\
Version 0.1 \
Aug 26, 2018 00:06 \
Author: Victor Akinwande 

Baseline. 

- Applied different multiclass classifiers using only the features at the finest scale (20 features).
- Stratified sampling of the training set with train-test ratio of 7:3
- Standard scaling: transforms the data such that its distribution has mean of 0 and standard deviation of 1
- Select 10 features based on their mutual information with the target
- Best model so far is a Support vector classifier with an RBF kernel

Selected features: `['NDVI', 'Mean_R', 'Mean_NIR', 'Bright', 'GLCM1', 'SD_R', 'SD_G', 'SD_NIR', 'Area', 'Mean_G']`


**Results on test set**

| Model        | No of Features          | Accuracy  |
| ------------- |:-------------:| -----:|
| SGD     | 20 | 0.7058823529411765 |
| SVC      | 20      |   0.6666666666666666 |
| Random forest | 20 |   0.5686274509803921  |
| KNN | 20 | 0.6274509803921569 |
| MLP | 20 | 0.7450980392156863 |
| MLP | 10 | 0.6666666666666666 |
| SVC | 10 | 0.7450980392156863 |

