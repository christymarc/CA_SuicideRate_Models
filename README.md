This repository includes the code for a linear regression model (ca_regression), a perceptron neural network (CA_SR_NeuralNet_73), and a convolutional neural network (CA_ConvNN_75) tasked with predicting the risk level of counties in California for high/low suicide rates based on a wide variety of demographical features.

A county's classified risk level for suicide is based upon its suicide rate with respect to the national suicide rate (13.42 per 100,000 individuals). If the county's rate exceeds the national average, it is classified as high risk; if the county's rate is below the national average, it is considered low risk. There are 33 demographical features in total that the models take into consideration. Some features include population, percentage of population with health insurance, percentage of population below the poverty line, percentage of population with a disability, percentage of population with veteran status, etc. Data on community features is from the U.S. Census Beauru, and data on county suicide is from the CDC. 

The repository also includes the trained models: CA_PNN_73 and CA_CNN_75. The models were trained on 20 California counties, which included the 10 counties with the highest suicide rate and the 10 counties with the lowest suicide rate. To test the models, a validation set of 37 California counties was used. CA_PNN_73 was able to predict county risk level for suicide with 72.97% accuracy and CA_CNN_75 was able to predict county risk level for suicide with 75.68% accuracy. The linear regression model predicted country risk with 67.57% accuracy.

All models are written in Python. The linear regression model uses Sklearn, and the neural networks use Pytorch.

In the "Old_Version_Old_Data" folder, there are previous versions of the models. These models used different U.S. Census Bureau data and made predictions based on only 10 demographical features. Also, the previous version of the regression model predicts suicide counts rather than risk level.

The "PEARC_Poster" pdf is a poster that summarizes this work. The poster was presented at ACM's Practice and Experience in Advanced Research Computing Conference in July of 2021.
