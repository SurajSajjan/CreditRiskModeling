# CreditRiskModeling

Machine Learning Model to predict the likelyhood of a customer defaulting his credit payment.

The dataset can be found from the following webiste - https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients.

Data Summary:

The dataset contains various attributes of the bank customers and if they defaulted payment of the previous month. 

Exploratory Data Analysis has been performed upon data wrangling. Feature engineering has been performed and Machine Learning Models have been build including Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, Adaptive Gradient Boosting and eXtreme Gradient Boosting. With an AUC socre of 0.77 in identifying Credit Defaulters, the Random Forest Classifier seems to be the best model in this Scenerio. This can be found in the notebook - CreditRiskAnalysis.ipynb

The Random Forest model has been saved as the "bestModel.pkl" pickle file. A falsk app is written using Swagger API to create a front end for the prediction model.   

A docker image is created containing all the required files and the docker image is pushed to an Azure Container Registry. A web app is created on Azure to run the Credit Risk Prediction Model.

The Docker file, the best model and other necessary files are in the folder - CreditRiskModelingDocker.