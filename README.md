# Neural_Network_Charity_Analysis

## Overview of the Analysis
The purpose of this analysis is to determine the impact of various donations from a philantrhopic organization, Alphabet Soup. Alphabet Soup is an organization that donates to other organizations that protect the environment, improve people's wellbeing, and unify the world. The CEO wants to find out which organizations are worth donating to and which are too risky. Using deep learning neural networks, this analysis provides an evaluation of all types of input to produce a clear, data-driven solution. 

## Results

### Data Preprocessing
* Target Variable: Is Successful
* Model Features: Status, Ask Amount, Application Type, Affiliation, Classification, Use Case, Organization, Income, Special Considerations
* Neither Target nor Feature: EIN, Name

### Compiling, Training, and Evaluating the Model
* Hidden Layer 1: 80
* Hidden Layer 2: 30
* "relu" activation function for both hidden layers
* "sigmoid" activcation function for output layer

This model reached an accuracy of 72.6%. This is below our target model performance, 75%. In order to increase model performance, I added one hidden layer, increased the number of neurons in one hidden layer, and changed activation to sigmoid for all layers. Additionally, I included the NAME column as a feature, rather than dropping it like in the original model. This model performed with an accuracy of 78.8%.

Before Optimization:

After Optimization:

## Summary
Overall, the original deep learning model was able to achieve of a performance of 72.6%. By adding a feature, adding another hidden layer, adding neurons to an exisiting hidden layer, and changing the activation functions, I was able to improve the model's performance to 78.8%. I also ran the model using the Random Forest Classifier. Using a different classifier can help to improve the model, which in this case it performed at 77.6%. I would recommend trying various classifiers as well as changing features and layers. 