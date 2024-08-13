# deep-learning-challenge
Module 21

Overview of the analysis: The purpose of this analysis is to train a modelt to predict if a donor's money will be used successfully based off of several factors.

# Data Preprocessing

* First I dropped the EIN and Name columns as they weren't relevant.  Then I determined the count of each application and determined to use the 'Is_Succesful' column for the model.
* Application types were changed to other for anything under 528 value counts
* Classification types were changed to other for anything under 1883 which was the cutoff for top 5.
* get_dummies was then used on the data for training.
* Is_succesful column was used for y and then dropped for the features and target arrays.


# Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why? I used 80 neurons on the first activation layer along with RELU, second hidden layer had 40 neurons and the output 
 layer was TANH.
* Were you able to achieve the target model performance? No...I was only able to get around 73% accuracy on the model.
* What steps did you take in your attempts to increase model performance?I added a 3rd hidden layer but in one case dropped the accuracy to under 50%, I raised the epochs to 150 and 200 with no effect.  I changed the neurons up and down but unable to attain 75%.  I changed the output from sigmoid to Tanh and that didn't have a large effect either.

