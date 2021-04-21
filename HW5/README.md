# HW 5

**Objective**: Implement a full end2end MLOps using wide and deep DNN model with proper feature engineering and preprocessing on the NYC Taxi Fare dataset from Kaggle. 

**Build with**:
* _**Tensorflow (EDA/VSA included)**_ (1) 
* _**Tensorflow with TFX**_ (2) 
* _**Pytorch**_ (3) 
* _**XGBoost**_ (4) 

**Feature Engineering**:
1. Haversine Distance
2. Distance to nearby Airports (JFK, EWR, LGR)

**Techniques applied**:
1. One-Hot encode all categorical attributes
2. Feature cross - Cross-join categorical attributes (ex: Lat cross Lon)
3. Network architecture - Wide (Categorical) and Deep (Continuous features)
4. Regularization(Overfit prevention) - L2
5. Uses GPU/TPU as distribution infrastructure 

**Highest Testing Accuracy Achieved**:
* **Tensorflow** (Train RMSE = 3.7527, Testing RMSE = 4.8123):
  - 25k training data, MSE Loss, ReLU Activation, Adam Optimizer, Learning Rate = 0.001, Number of Epoch = 50
* **Tensorflow with TFX** (Train RMSE = 5.8757, Testing RMSE = 3.7620): 
  - 3 Hidden Layer, MSE Loss, ReLU Activation, Adam Optimizer, Learning Rate = 1e-05, Number of Epoch = 50
* **Pytorch** (Train RMSE = 5.5701 , Testing RMSE = 4.8073):  
  - MSE Loss, ReLU Activation, Adam Optimizer, Learning Rate = 1e-2, Number of Epoch = 100
* **XGBoost** (Train RMSE = 2.5046, Testing RMSE = 3.8093):  
  - Early stopping, Max Depth = 8, Gamma = 0, ETA = 0.05

Reference/Modified code from the following notebooks: 
* https://colab.research.google.com/drive/1xS2YjhCYGnOrsyVRKxqN-PvdFROSnDvM?authuser=1#scrollTo=fK9LdIbXN87L
* https://colab.research.google.com/gist/rafiqhasan/2164304ede002f4a8bfe56e5434e1a34/dl-e2e-taxi-dataset-tfx-e2e.ipynb
