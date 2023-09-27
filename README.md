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
neural network using TensorFlow's Keras Sequential API.
It consists of 2 hidden layers and 1 output layer.

•	First model neural network using TensorFlow's Keras Sequential API. It consists of 4 hidden layers and 1 output layer. 
First hidden layer: number_input_features*3 neurons. Swish activation.
Second hidden layer: number_input_features*2 neurons. ReLU (Rectified Linear Unit) activation.
Additional hidden layer: number_input_features neurons.ReLU activation.
Output layer: 1 neuron (since it's a binary classification).Sigmoid activation (suitable for binary classification).

the model's validation accuracy of approximately 72.52% and a validation loss of 0.5547 in its final epoch.
Accuracy: The model achieved a final accuracy of approximately 72.52% on the validation set.
Loss: The binary cross-entropy loss was approximately 0.5547 on the validation set.