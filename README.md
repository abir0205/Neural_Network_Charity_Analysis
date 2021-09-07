# Neural_Network_Charity_Analysis

## Overview of Analysis
The purpose of this project is to create a deep learning neural network model using TensorFlow to evaluate whether the model can predict the whether an organization will receive funding from Alphabet Soup. A CSV file of the metadata was provided to use as the parameters to feed the neural net. An ideal model would be able to predict whether or not a organization would receive funding from Alphabet Soup.

## Results
### Data Preprocessing
- For this model, the IS_SUCCESSFUL column of the CSV file was used as the target variable. This column was already presented in a binary notation and was indicative of whether funding was used successfully or not.
- The columns containing EIN and NAME were removed when analyzing the data as they provided no use to the neural net.
- All other columns were used as features for the neural net.


### Compiling, Training, and Evaluating the Model
- For the initial model, deep learning neural net with two hidden layers was created, with hidden layer 1 containing 80 neurons and hidden layer 2 containing 30 neurons. A Rectified Linear Unit (ReLU) activation function was used for both layers as this is considered standard for these types of neural nets. A sigmoid activation was used for the output activation due to the binary nature of the results, as they would always be 0 or 1.
- For the initial model, an accuracy of 73.08% was calculated.
- To optimize these results for further neural nets, a variety of methods was used. This included adding another hidden layer, adding more neurons to each hidden layer, changing the activation function in the hidden layers to leaky ReLU, and lowering the threshold for bins for lower counts. However, the accuracy of these models never rose above 74%, below the ideal threshold of 75% accuracy.

## Summary
- The models were capable of predicting the outcome of a majority of the organizations receiving funding but was never able to go above the 75% accuracy threshold, meaning that this model is not optimal and is not overperforming. Further work needs to be done in order to create a more accurate model which can predict this data. It may be more beneficial to use a random forest classifier as opposed to a deep learning model due to the fact random forest classifiers are known to have similar levels of accuracy as deep learning models but are easier to build and analyze.
