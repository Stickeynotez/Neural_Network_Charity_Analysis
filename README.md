# Neural_Network_Charity_Analysis

## Overview
This project uses neural networks and deep learning to predict whether applicants will be successful if funded by AlphabetSoup or not.

## Results 
### Data Preprocessing

Going in order 
Two columns were removed from the dataset, EIN and NAME, as they are not resourceful to the analysis at hand.
The remaining columns are as follows.

![image](https://user-images.githubusercontent.com/99559096/182273715-c30df85f-814e-49b0-9cb1-d7cb3219abd6.png)

There are two more columns with more than 10 unique values, where binning was used on these columns prior to encoding for analysis.
Our primary objective of this model is to veirfy if an applicant will be successful if funded or not. This makes the target variable the "IS_SUCCESSFUL" column.

### Compiling, Training, and Evaluating

In my non-optimized neural network, I started with 8 neurons in layer 1 and 5 neurons in layer 2. Throughout my reading/experience, the more neurons a model has, the less efficient it becomes, with more neurons overfitting also occurs. 

![image](https://user-images.githubusercontent.com/99559096/182497624-437b387e-d98d-41c0-9a0f-11102af51b24.png)

The model produced a predictive accuracy of 72.36%, this is far from the 75% target.

### Optimization

I started the optimization process by cleaning the dataset more, removing seemingly unneccesary rows. 
STATUS column was the first to go. - This did not increase accuracy significantly

From here I added another hidden layer to my model - and added more neurons to each layer
Layer 1 has 220
Layer 2 has 180
Layer 3 has 160
I also changed one of the activation functions from relU to tanh

![image](https://user-images.githubusercontent.com/99559096/182498054-41baa85f-ce79-4350-b166-b89709d1a1dd.png)

From that point I hadded more neurons to my model which is where we are now. 

![image](https://user-images.githubusercontent.com/99559096/182498088-d2fe9e4c-1d44-4adf-b0af-b2914682aa5e.png)

Adding the large amount of neurons, and changing the activation function seemed to have little to no effect on the overall accuracy.

# Summary
Overall, both models produced a 72.XX% accuracy score using this model, although in some cases 72% accuracy is considered to be a fairly precise measurement, in the case of monetary value and risk, 72% is not effective for predicting if a company will succeed or not. Another model that may be better for this application would be RandomForest, or the K-Means test.
