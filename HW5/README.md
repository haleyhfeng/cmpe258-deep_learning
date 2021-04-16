# HW 5

**Objective**: Implement a full end2end MLOps using wide and deep DNN model with proper feature engineering and preprocessing on the NYC taxi dataset. 

**Build with**:
* _**Tensorflow (with EDA/VSA included)**_ (1) 
* _**Tensorflow with TFX**_ (2) 
* _**Pytorch**_ (3) 
* _**XGBoost**_ (4) 

**Techniques applied**:
1. One-Hot encode all categorical attributes
2. Feature cross: Cross-join categorical attributes( ex: Lat cross Lon )
3. Network architecture: Wide( Categorical ) and Deep( Continuous features )
4. Regularization( Overfit prevention ): L2
5. Uses GPU / TPU as distribution infrastructure 

**Highest Testing Accuracy Achieved**:
* **Tensorflow** (Train RMSE = , Testing RMSE = ): 
* **Tensorflow with TFX** (Train RMSE = , Testing RMSE = ):  
* **Pytorch** (Train RMSE = , Testing RMSE = ):  
* **XGBoost** (Train RMSE = , Testing RMSE = ):  

Reference/Modified code from the following notebooks: 
* https://colab.research.google.com/drive/1xS2YjhCYGnOrsyVRKxqN-PvdFROSnDvM?authuser=1#scrollTo=fK9LdIbXN87L
