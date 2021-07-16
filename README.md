# Neural Network Charity Analysis

## Overview
The purpose of this assignment was to create a neural network to predict where to make investments by Alphabet Soup. The goal was to use the provided dataset of over 34,000 organizations that have received funding from Alphabet Soup and to use the information to predict whether applicants will be successful if funded by Alphabet Soup.
## Results
 - Data Preprocessing
	- The target variable for my model was the IS_SUCCESSFUL column
	- The features in the model are APPLICATION_TYPE, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT
	- I think ASK_AMT is neither a variable or feature so I removed it during optimization
 - Compiling, Training, and Evaluating the Model
	- I used two hidden layers, with the first layer having 80 neurons and the second layer having 30 neurons. Since we had 43 features, I wanted to do the 2x rule for number of neurons. Originally, the RELU/Sigmoid activations were used. 
	- I was not able to reach the target model performance with any of the changes that I made. 
	- My first attempt was to remove the ASK_AMT column

	- My second attempt was to increase the neurons from 80/30 to 100/60

	- My third attempt was to change the sigmoid output activation to TANH
	
	
## Summary
After three attempts I was not able to reach the target model. This may be because I was overfitting the data due to removing too many columns. Changing the neurons and the activation layer seemed to make the accuracy lower, so I am guessing I was overfitting the data. I would need to research more about what columns would really be needed and how best to bin items to make more sense. I also need more experience with choosing the correct activation layers and they are not totally clear to me.