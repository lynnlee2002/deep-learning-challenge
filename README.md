# deep-learning-challenge
1) Overview of the analysis:
   This analysis is to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. The raw data was first preprocessed using Pandas and Scikit-Learn's tools to later split the data into training and testing datasets. The training and testing datasets are then scaled with StandardScaler instance, fit into the training data, then tranformed using the 'transform' function.
  A binary classification model (or deep learning model) was designed using TensorFlow and a neural network approach. The number of input features was determined based on the preprocessed dataset, and a sequential model was created with multiple layers.

2) Results:
   - The target variable for the model is the "IS_SUCCESSFUL" columns - was the money used effectively - in the dataset. It indicates whether or not an application is successful if funded by Alphabet Soup.
   - The features for the model are all the columns in the dataset except for the target variable:
     + APPLICATION_TYPE — Alphabet Soup application type
     + AFFILIATION — Affiliated sector of industry
     + CLASSIFICATION — Government organization classification
     + USE_CASE — Use case for funding
     + ORGANIZATION — Organization type
     + STATUS — Active status
     + INCOME_AMT — Income classification
     + SPECIAL_CONSIDERATIONS — Special considerations for application
     + ASK_AMT — Funding amount requested
  - Variables should be removed from the input data because they are neither targets nor features:
     + EIN and NAME—Identification columns
  - Number of neurons:
     + Hidden layer 1: 80
     + Hidden layer 2: 30
     + Output Layer: 1 neuron (for binary classification)
  - The target model performance of higher than 75% accuracy was not achieved.
  - To increase model performance, I adjusted the number of hidden layers and neurons in each hidden layer, and epochs.
