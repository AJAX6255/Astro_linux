# Classification of Type II Cepheids 

## Required packages:
astropy,
pandas,
upsilon,
seaborn,
pickle,
urllib,
sklearn,
FATS -- available on https://github.com/isadoranun/FATS
<br />

## Folders and Files
#### time_series_analysis
The file "LX_Cyg.ipynb" is a tutorial showing how to plot the raw data, a periodogram, and phase plot.
#### feature_extraction
This folder goes over the process of extracting features from the raw data and storing them in an SQL database.  The file "feature_extraction.ipynb" is using a Python 2.7 kernel.  It is important to note that every other .ipynb file in this repository is using a Python 3.x kernel.
#### classification
This folder goes over the steps involved to make the classifier "voting_ensemble_without_colour.pickle".  This includes data visualization, outlier detection and removal, feature scaling, principal component analysis, tuning the hyper-parameters of a model, and evaluating the goodness of the classifier.
#### classifier_finished
This folder demonstrates how to use the classifier.  Place the raw data files in the folder "Time_Series".  Each raw data file must include the columns time, magnitude, and error which are separated by a space.  Then run scripts "1. feature_extraction.ipynb" and "2. classification.ipynb", respectively.
#### machine_learning_notes.pdf
These notes are intended to provide some intuition and mathematical background to the machine learning techniques that were used to make the classifier.
