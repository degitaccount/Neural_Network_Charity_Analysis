# Neural_Network_Charity_Analysis

## **Overview**

This analysis uses deep learning neural networks to predict whether applicants receiving charitable donations will have successful campaigns.

## Results

### Data Processing
* “IS_SUCCESFUL” is the target for this model since it flags the success of previous donations.

*	This model contains 9 features: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.

*  EIN and NAME were deleted from the dataset since they were not beneficial to the analysis – these data points are not considered model features nor targets.

### Compiling, Training and Evaluating the Model
This deep-learning model contains two hidden layers, one with 80 neurons and another with 30 neurons. 

* Each hidden layer was activated with the more complex relu algorithm while the outer layer was activated with the sigmoid algorithm since its output represents probability.  

* The adam optimizer and binary_crossentropy were used to compile the model.

After three attempts to improve the model’s performance, the accuracy remained below the target of 75%.  The changes to the original model included:

* Adding a third a hidden layer

* Changed the activation method from “relu” to “tanh”

* Changed the optimizer in the model compilation from “adam” to “nadam”

All three changes reduced he model's acccuracy.

## Summary
The model did not achieve the target accuracy of 75%, even after three attempts to improve its performance.  Since the target accuracy level is not striving for perfection, a supervised machine learning model could be a simpler solution for evaluating the potential success of specific charitable donations.
