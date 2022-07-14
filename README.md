# Project2

## Data: SARS and FDIC Quarterly Banking Profile 
    - SARS for Depository Institutions 2014-2021: [Resources/SARStats2014_2021.csv](Resources/SARStats2014_2021.csv) <br>
    - FDIC Quarterly Banking Profiles: [Resources/FDICQBPs.csv](Resources/FDICQBPs.csv)<br>
Data cleaning process: [data.ipynb](data.ipynb)
## Overview
Using the data we gathered, we wanted to see if we can create a predictive model to predict the next quarter's Depository Institution fraud reporting number based on the Net Operating Income from FDIC Quarterly Banking Profiles. We decided to do 4 different models, **Decision Tree, Random Forest and 2 Deep learning models**

## Code
[Decision Tree](decision_tree_H.ipynb)<br>
[Random Forest](random_forest.ipynb)<br>
[LSTM RNN Model 1](deep_tensorflow_wj.ipynb)<br>
[LSTM RNN Model 2](deep_learning_as.ipynb)<br>

## Outputs
### Decision Tree
Using a decision tree model, we were able to create the following tree:
![Resources/Images/decision_tree.png](Resources/Images/decision_tree.png)

**The R squared score we got with this model was: 0.656673881135426**<br>
**Resulting Plot:**<br>
![Resources/Images/HakobDTOutputPlot.png](Resources/Images/HakobDTOutputPlot.png)

### Random Forest 
Using Random Forest, we tried first with all the features and got the following feature importances: <br>
![Resources/Images/RandomForestAllFeatureImportances.png](Resources/Images/RandomForestAllFeatureImportances.png)<br>
However the R2 score was pretty low, so we took out some features and ended up with<br>
![Resources/Images/RandomForestFeatureImportances.png](Resources/Images/RandomForestFeatureImportances.png)<br>
**The R squared score we got with this model was: 0.6367452319814639**<br>
**Resulting Plot:**<br>
![Resources/Images/RannyRFOutputPlot.png](Resources/Images/RannyRFOutputPlot.png)<br>

### LSTM RNN Model 1
Summary of Model 1:<br>
![Resources/Images/Model1Summary.png](Resources/Images/Model1Summary.png)<br>
**The R squared score we got with this model was: 0.56**<br>
**Resulting Plot:**<br>
![Resources/Images/WadeehaModelOutputPlot.png](Resources/Images/WadeehaModelOutputPlot.png)<br>

### LSTM RNN Model 2 
Summary of Model 2:<br>
![Resources/Images/Model2Summary.png](Resources/Images/Model2Summary.png)<br>
**The R squared score we got with this model was: 0.839697950645499**<br>
**Resulting Plot:**<br>
![Resources/Images/AkankshaModelOutputPlot.png](Resources/Images/AkankshaModelOutputPlot.png)<br>
