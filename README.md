Alphabet Soup- Successful Funding Prediction Model


Overview: The purpose of this analysis is to create an algorithm which will predict
whether or not applicants for funding will be successful in their use of that funding.
Process: Alphabet Soup provided a CSV with historical data on more than 34,000
organizations including their name, EIN, application type, industry affiliation,
government organization classification, use case for funding, organization type,
active status, income classification, special considerations, the funding amount
requested and was the funding used effectively. The target variable for the model is
successful funding and the remaining variables , excluding the EIN and name, are the
features.

![image](https://user-images.githubusercontent.com/86893003/161859870-3ac5f1cc-9a77-4307-a02d-27b12e87937c.png)

![image](https://user-images.githubusercontent.com/86893003/161861078-27d0ca77-b40b-4edb-890f-8dbf38d4883d.png)



Compiling, Training and Evaluating the Model: I started with two dense layers with 200
neurons in each layer using a sigmoid activation function. I chose the sigmoid activation
function because the model is intended to predict a yes/no outcome. That is there are only
possible outcomes and the probability exists between 0 and 1. The model was run for 50
epochs.

![image](https://user-images.githubusercontent.com/86893003/161861127-b4cf27f1-c4ce-4bf8-944b-8b3d0583fef7.png)


The model achieved an accuracy rate of 72.54%, which is below the target of 75%. I first tried
adding a third layer of 100 neurons. This decreased the model accuracy slightly to 72.37%. I
then went back to 2 layers and increased the number of neurons. This was also slightly less
accurate than the original model, with an accuracy rate of 72.51%. My final attempt was to run
the model with 2 layers of 200 neurons for 100 epochs instead of 50. This lead to a very slight
increase in accuracy, 72.57%. The model never achieved the desired accuracy rate.


Summary: Overall, this model was about 72% accurate. If I were to work on it further I would
try changing the input values to see if I could find one that had more salience for the mod
