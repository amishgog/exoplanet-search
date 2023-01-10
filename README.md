# Description
This is a project which aims at using Machine Learning and Python to execute a model and search for exoplanets around G-Type stars. We use light transit data from the Transiting Exoplanet Survey Satellite (TESS) to construct light curves. Features were extracted from these light curves and fed into machine learning algorithm and the predictions were printed. 

# Tools used
1) lightkurve package was used to construct light curves
2) pandas used for data framee creation
3) tsfresh used for time series (light curve) feature extraction
4) sklearn used for application of data pre-processing and ML algorthim

# Brief Overview
We first upload csv files taken from the NASA Exoplanet Archive and Mikulski Archive for Space Telescopes (MAST) which contains IDs for stars. We use lighkurve package to access pixel files from MAST data. We then construct light curves from these pixel files using the lightkurve package. These light curves are tranformed to csvs and used to extract features which are then put in a single csv files for all stars. We then use tools like normalization, Sampling and Principle Component Analysis (PCA) to pre-process our data for training and testing the ML algorithm. When the final result in printed we append this array into an new file with Star IDs which were analysed and the prediction for existance of exoplanets as a Boolean.
