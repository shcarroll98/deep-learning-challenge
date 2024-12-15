Overview:

In this analysis I develop and evaluate a deep learning model for predicting charitable donations. The goal is to find potential donors based on characteristics derived from historical donation data.

Results:

The target variable for the model is the binary indicator of whether someone donates to charity from the column ‘Donation_Status’.

The feature variables include income, age, gender, education, marital status, number of children, home ownership, employment status, annual gift amount. We removed ID and EIN since these are not attributes we evaluate in correlation to donation status. 

The model architecture has an input layer based on the nine features. It has 2 hidden layers using the ReLU activation function. The first hidden layer has 80 neurons, the second hidden layer has 30 neurons. 

The output layer uses the Sigmoid activation function and has an output layer of 1 neuron.

The choice of 80 neurons in the first layer and 30 neurons in the second layer balances complexity and efficiency. ReLU activation is good for handling non-linearity. 

Model Performance:

Final Training Accuracy:  74.16%
Final Test Accuracy: 72.63%

The final model achieved an accuracy of 74.16% on the training set and 72.63% on the test set, indicating good generalization performance.

Recommendation: As far as an alternative model, a random forest classifier can handle a large number of features and their interaction without requiring feature scaling. Performance of the predictive model could be further enhanced by exploring an alternative model and fine-tuning the neural network.

