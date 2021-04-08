# HW 4

**Objective**: Build a Feed Forward Neural Network to train on MNIST dataset.

**Build with**:
* _**Pure Numpy**_ (1) 
* _**Pure Keras, Tensorflow (Custom Subclass)**_ (2) 

**Techniques applied**:
* **Mini-Batch Gradient Descent** 
* **Dropout Regularization Layer**
* **Appropriate Weight Initialization** 
* **Image Augmentation with Keras Preprocessing**
* **Tuning of Number of Neurons and Layers**
* **ReLU Activation Layer**
* **Normalization** 
* **Appropriate/Adaptive Learning Rate** 
* **Visualization, Confusion Matrix** 

**Highest Accuracy Achieved**:
* **Numpy** (Train Acc = 99.77%, Testing Acc = 97.02% ): 
    - Randomly select 10k training data + extra 30k augmented, 4-layers NN [784, 200, 80, 10], MSE Loss, ReLU Activation, Mini-Batch GD with Batch Size 256, Learning Rate = 0.016, Number of Epoch = 401
* **Keras** (Train Acc = 97.72% , Testing Acc = 97.44% ):  
    - Randomly select 10k training data, 4-layers NN [784, 200, 80, 10], MSE Loss, ReLU Activation, Adam Optimization, Mini-Batch ImageDataGenerator Batch Size 512, Learning Rate = 0.001, Number of Epoch = 401


Reference/Modified code from the following notebooks: 
* https://colab.research.google.com/drive/1HS3qbHArkqFlImT2KnF5pcMCz7ueHNvY?authuser=1#scrollTo=Wo5zDlScdl4s 
* https://colab.research.google.com/drive/17u-pRZJnKN0gO5XZmq8n5A2bKGrfKEUg#scrollTo=67-lEi5tjYwd 
* https://www.kaggle.com/yassineghouzam/introduction-to-cnn-keras-0-997-top-6 
* https://github.com/iamtrask/Grokking-Deep-Learning/blob/master/Chapter9%20-%20Intro%20to%20Activation%20Functions%20-%20Modeling%20Probabilities.ipynb
