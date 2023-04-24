# Land-Cover-Prediction-Using-Machine-Learning

Climate change has become a serious threat to humanity. Global land cover maps serve as an important
means to tackle this problem. ESA has produced Global Land Cover Map from Sentinel-2 data. 
In this project, land cover maps were generated for  unseen data by using a limited number of training samples. Gibraltar is selected as a study area as there are wide variety of land cover types.

<img src="https://github.com/iremozcann/Land-Cover-Prediction-Using-Machine-Learning/blob/main/images_for_readme/data1.png" alt="alt text" width="600">


## About Data Files
- Original data files are TIFF image files. They are in 2D spatial files. Numpy and CSV files are converted to suitable formats for SKLearn classifiers
- Train.csv contains both Labels(Code) and Data. Test.csv contains only test data.
- Data is UInt16, and Classlabels are Uint8.
- Training data: S2A_MSIL1C_20220516_TrainingData.tif
- Training labels: S2A_MSIL1C_20220516_Train_GT.tif
- Test: S2B_MSIL1C_20220528_Test.tif
- Class List:

<img src="https://github.com/iremozcann/Land-Cover-Prediction-Using-Machine-Learning/blob/main/images_for_readme/class-list.png" alt="alt text" width="400">

Reference: https://esa-worldcover.s3.eu-central-1.amazonaws.com/v200/2021/docs/WorldCover_PUM_V2.0.pdf

*Note: If you open CSV files with Excel It will truncate data exceeding 1 million'th row.*

### Land Cover Map from Sentinel-2 data
Each Sentinel-2 satellite is equipped with a single multi-spectral instrument (MSI) that has 13 spectral channels in the visible/near infrared (VNIR) and short-wave infrared (SWIR) spectrums.
Continued collaboration with the SPOT-5 and Landsat-8 missions is possible inside the 13 bands thanks to the 10-meter spatial resolution, with a primary goal of land classification.

## Machine Learning Methods
The objective of the project is to
estimate the land-cover changes by
employing machine learning techniques.In this study, various machine learning techniques
such as Random Forest, K- Nearest Neighbor ( KNN) has been used for
land cover prediction from satellite imagery. Furthermore,
user-defined hyperparameters are optimized to obtain higher
accuracy results. The Grid Search method was used to find the best
parameters of each algorithm. Additionally, the k-fold cross-validation approach (k = 10, iteration = 10) is employed to obtain more precise and objective results.
