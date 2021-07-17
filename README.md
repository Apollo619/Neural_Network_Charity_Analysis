# Neural Network Charity Analysis

## Overview of Analysis
I am tasked with helping **Beks**, a data scientist and programmer for the non-profit organization ***Alphabet Soup*** with determining the impact of donations it makes to other organizations. 

### Purpose:
Using our knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help **Beks** create a binary classifier that can predict whether applicants will be successful if funded by ***Alphabet Soup***.

## Results: 

The CSV contains various data (see image below) on more than 34,000 organizations that have received funding from ***Alphabet Soup*** over the years. We will perform **preprocessing**, **compiling**, **training**, and **evaluating** for our Machine Learning (ML) model.  Please read bullets below for common ML questions and answers. 
![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/dataset.PNG)

1. *Data Preprocessing*
  - What variable(s) are neither target nor features, and should be removed from the input data? 
    - One of the first things done is to remove the columns for the organization name and EIN as they are non-beneficial ID’s and provide no usable input for ML. See image below       for code used to remove these columns.  

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/non-beneficial.PNG)

   - What variable(s) are the features for your model?
     - Next is to identify which columns will be features (see below image) or data that will be fed into the algorithms to perform the ML. 

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/features.PNG)

   - What variable(s) are considered the target(s) for your model?
     - And lastly, for the preprocessing we must determine which column will be used as the target (see image below) to train the feature data to help predict if an organization        will be considered ***”successful”*** if donations are provided. 

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/target.PNG)

2. *Compiling, Training, and Evaluating the Model*
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - 100, 70, 50, and 20 neurons over 4 layers using the activation function “relu” was selected for the neural network model. With this munch data is seemed logical to add           more neuron and layers from the recommendation of the challenge assignment. See image below for visualization of neurons and layers. 

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/Neurons%20and%20Layers.PNG)

  - Were you able to achieve the target model performance?
    - I was able to achieve ~72% accuracy (see image below) with the neural network model. Depending on level of accuracy this can be considered accurate except the “loss” is abnormally high at ~55% making the model not as accurate as we would hope. 

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/accuracy.PNG)

  - What steps did you take to try and increase model performance?
    - A multitude of steps were taken to try and increase the model performance. 
    - One, changing how certain columns were binned as shown in the below images.

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/binning1.PNG)

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/binning.PNG)

   - Next, two additional layers and increasing the number of neurons used in the ML model. See images below. 

![](https://github.com/Apollo619/Neural_Network_Charity_Analysis/blob/main/Resources/changes.PNG)

   - Lastly, I tried changing the “activation” from relu to tanh with no increase in accuracy observed. (see above image) 
		

## Summary:

Based on the neural network model it would be difficult to provide an accurate prediction of organization and if they can be considered ***”successful”*** if **Alphabet Soup** provides donations. 

Unfortunately, at this time no recommendation can be ascertained unless additional time to evaluate the model can be done. 
