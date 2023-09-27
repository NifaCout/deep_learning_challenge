# deep_learning_challenge
Deep learning 
Introduction: 
Neural Network Model Analysis for Alphabet Soup
Alphabet Soup is a nonprofit foundation dedicated to supporting various organizations with funding. Over the years, they have supported more than 34,000 organizations, to ensure that the funds are used efficiently and produce the desired impact, there's a pressing requirement to predict which organizations are more likely to succeed in their ventures when supported. 
Purpose: 
The primary goal of this analysis is to leverage the dataset to create a binary classifier, utilizing machine learning and neural networks. This classifier aims to predict the likelihood of an applicant's success if funded by Alphabet Soup. By achieving this, Alphabet Soup can make more informed decisions, thereby ensuring that their funds make the most significant possible impact.

Data Preprocessing:
'IS_SUCCESSFUL' is a Target Variable which indicates whether an organization was successful in effectively using the funds they received from Alphabet Soup. It's a binary variable where a value (e.g., 1) might indicate success, and another value (e.g., 0). the neural network model, predicting this binary outcome will guide funding decisions, ensuring resources are allocated to applicants with a higher likelihood of success.

Compiling, Training, and Evaluating the Model:
•	First model neural network using TensorFlow's Keras Sequential API. 
Contains 4 hidden layers and 1 output layer: 
    First hidden layer: number_input_features*3 neurons. Swish activation.
    Second hidden layer: number_input_features*2 neurons. ReLU (Rectified Linear Unit) activation.
    Additional hidden layer: number_input_features neurons.ReLU activation.
    Output layer: 1 neuron (since it's a binary classification).Sigmoid activation (suitable for binary classification).
Performance Metrics:Validation Accuracy: Approximately 72.52% and Validation Loss: Approximately 0.5547.

•	Second model neural network using TensorFlow's Keras Sequential API.
Contains 3 hidden layers and 1 output layer.
    First hidden layer: number_input_features*3 neurons with Swish activation.
    Second hidden layer: number_input_features*2 neurons with ReLU activation.
    Additional hidden layer: number_input_features neurons with ReLU activation.
    Output layer: 1 neuron with Sigmoid activation (for binary classification).
Optimizer: Adam with a learning rate of 0.001. Epochs: 100 and Batch size: 32
Performance Metrics Validation Loss: 0.5903, Validation Accuracy: 72.2%.

•	Third model neural network using TensorFlow's Keras Sequential API.
Contains 3 hidden layers and 1 output layer:
    First hidden layer: number_input_features*3 neurons with Swish activation and L2 regularization. Additionally, a dropout rate of 20%.
    Second hidden layer: number_input_features*2 neurons with ReLU activation and L2 regularization. Again, a dropout rate of 20%.
    Additional hidden layer: 
        number_input_features neurons with ReLU activation.
        Output layer: 1 neuron with Sigmoid activation (for binary classification).
Optimizer: Adam with a learning rate of 0.001. Callbacks: Early stopping based on validation loss with  patience of 10 epochs. Epochs: Not specified due to early stopping callback and Batch size: 32
Performance Metrics: Test data evaluation:Loss: 0.57%.Accuracy: 72.43%.

The three models each trying to optimize the performance of a neural network on the dataset. The differences in performance metrics among them are subtle. Model 3: L2 regularization techniques and dropout helped eliminate overfitting from the Second Model.
