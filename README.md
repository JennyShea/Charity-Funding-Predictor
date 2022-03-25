Background
The non-profit foundation Alphabet Soup wants to create an algorithm to predict whether or not applicants for funding will be successful. Create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:


EIN and NAME—Identification columns

APPLICATION_TYPE—Alphabet Soup application type

AFFILIATION—Affiliated sector of industry

CLASSIFICATION—Government organization classification

USE_CASE—Use case for funding

ORGANIZATION—Organization type

STATUS—Active status

INCOME_AMT—Income classification

SPECIAL_CONSIDERATIONS—Special consideration for application

ASK_AMT—Funding amount requested

IS_SUCCESSFUL—Was the money used effectively


Instructions

Step 1: Preprocess the data
Using your knowledge of Pandas and the Scikit-Learn’s StandardScaler(),  preprocess the dataset in order to compile, train, and evaluate the neural network model later in Step 2

Read in the charity_data.csv to a Pandas DataFrame, and identify the following:

What variable(s) are considered the target(s)?
What variable(s) are considered the feature(s)?


Drop the EIN and NAME columns.
Determine the number of unique values for each column.
For those columns that have more than 10 unique values, determine the number of data points for each unique value.
Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.
Use pd.get_dummies() to encode categorical variables


Step 2: Compile, Train, and Evaluate the Model
Using TensorFlow,  design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. Compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

Continue using the jupter notebook where you’ve already performed the preprocessing steps from Step 1.
Create a neural network model by assigning the number of input features and nodes for each layer using Tensorflow Keras.
Create the first hidden layer and choose an appropriate activation function.
If necessary, add a second hidden layer with an appropriate activation function.
Create an output layer with an appropriate activation function.
Check the structure of the model.
Compile and train the model.
Create a callback that saves the model's weights every 5 epochs.
Evaluate the model using the test data to determine the loss and accuracy.
Save and export your results to an HDF5 file, and name it AlphabetSoupCharity.h5.


Step 3: Optimize the Model
Using your knowledge of TensorFlow, optimize your model in order to achieve a target predictive accuracy higher than 75%. If you can't achieve an accuracy higher than 75%, you'll need to make at least three attempts to do so.
Optimize your model in order to achieve a target predictive accuracy higher than 75%. 


Report on the Neural Network Model including recommendations for future models


