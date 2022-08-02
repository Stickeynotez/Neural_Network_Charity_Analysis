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
