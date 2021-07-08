# Neural_Network_Charity_Analysis
This project will use neural network models to predict whether the nonprofits that my client's company donates to will use their donated money effectively. 

## Overview of the analysis
The purpose of this project is to aid my client, Alphabet Soup, in determining which nonprofits will use their donated money for good. The machine learning model will use neural network models to predict if a nonprofit will be successful after receiving donations from Alphabet Soup. 

## Results:

### Data Preprocessing
#### What variable(s) are considered the target(s) for your model?
The target/dependent column will be the ‘IS_SUCCESSFUL’ column. The model will predict whether the nonprofit will be successful based on the independent/feature columns.
[target screenshot]

#### What variable(s) are considered to be the features for your model?
The features/independent columns are ‘APPLICATION_TYPE’, ‘AFFILIATION’, ‘CLASSIFICATION’, ‘USE_CASE’, ‘ORGANIZATION’, ‘STATUS’, ‘INCOME_AMT’, ‘SPECIAL_CONSIDERATIONS’, ‘and ‘ASK_AMT’
[features screenshot]

#### What variable(s) are neither targets nor features, and should be removed from the input data?
The columns which would make no impact on the target are the ‘EIN’ and ‘NAME’ columns
[dropping columns screenshot]

### Compiling, Training, and Evaluating the Model
#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
I created one hidden layer with 80 neurons and another with 48. I used a relatively low amount of neurons and only two hidden layers to avoid overfitting of the model. I used the ‘relu’ activation function so the model could look for any non-linear and linear patterns.
[nn_model screenshot]

#### Were you able to achieve the target model performance?
Although I altered the model, I was not able to achieve the target model performance.
[accuracy_loss screenshot]

#### What steps did you take to try and increase model performance?
The steps I took were to avoid overfitting the model. I lowered the number of neurons, epochs, and features. Additionally, I decreased the number features to avoid providing more data than necessary to the model. 

## Summary
The deep learning model predicted approximately 61% of the data correctly. While in some cases, this may be adequate; for Alphabet Soup’s purpose, the percentage would need to be higher so they are not wasting money. In order to raise the prediction rate, I would recommend using auto-optimization. Using the auto-optimization model, we would be able to quickly see the number of neurons and hidden layers needed to get the most accurate results from the model. In addition, I would recommend viewing the metadata in order to see the columns that could be deleted from the features. 

In conclusion, the model created is a good start to creating accurate predictions. However, to help Alphabet Soup, we would need to adjust the model to allow for improvements, thus leading to further accurate results.

