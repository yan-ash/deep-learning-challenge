# deep-learning-challenge Report

### Purpose of the analysis:

I've created a tool for the nonprofit foundation Alphabet Soup that can help it select applicants for funding with the best chance of success in their ventures. Using my knowledge of machine learning and neural networks, I have used the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

### Step 1: Preprocess the Data

1. Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset

1. Target Varible of the model ----IS_SUCCESSFUL
1. Feature Variables for the model:
   APPLICATION_TYPE
   AFFILIATION
   CLASSIFICATION
   USE_CASE
   ORGANIZATION
   STATUS
   INCOME_AMT
   SPECIAL_CONSIDERATIONS
   ASK_AMT

### Step 2 : Compile, Train and Evaluate the Module

1. Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.
![image](https://user-images.githubusercontent.com/109451707/211553499-25fb47b6-0cca-4f88-bb2b-e40cf8bc147d.png)

1. hidden layers with 80, 30 neurons split (the input (node) feature was 43, 80 was chosen as the first layer as it is almost double the input_feature). With an hidden layer activation function of relu as this our go to for first model.
   Output node is 1 as it was binary classifier model with only one output: was the funding application succesfull yes or no. And an output layer activation of sigmoid as the model output is binary classification between 0 and 1.

1. Compile and train the model.
1. Evaluate the model using the test data to determine the loss and accuracy.
![image](https://user-images.githubusercontent.com/109451707/211553596-06345dd3-daa4-4fe9-8174-a5b610a7f781.png)

1. Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity.h5

### Step 3: Optimise the Model

I experimented with increasing nodes and neurons, with changing other parameters to get a better accuracy but despite doing this both models came below the 75% threshold.

### Conclusion :

No matter I dropped another column or binning more rare orrurences in the column, I could not managed to get a better result.

I have added more neurons to a hidden lay and increase the epochs, the result would not appear to be improving.
