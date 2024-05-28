# deep_learning_challenge
Module 21


# Overview: 
We have a set of data for charity events that were successful.  We are looking to train a model to predict if future events will be successful or not with at least 75% accuracy.

# Results
## Data Preprocessing
o	What variable(s) are the target(s) for your model?

The target variable is the "IS_SUCCESSFUL" column.

o	What variable(s) are the features for your model?

All of the other columns except for EIN and NAME.

o	What variable(s) should be removed from the input data because they are neither targets nor features?

EIN and NAME are removed as they do not provide data to help the model predictions.

## Compiling, Training, and Evaluating the Model
o	How many neurons, layers, and activation functions did you select for your neural network model, and why?

I ran several iterations as follows:

Start - 2 layers, 8 and 5 neurons, relu and sigmoid output

Opt1 - kerastuner, 5 layers, 17,67,1,43,76, tanh and sigmoid output

Opt2 - kerastuner, 5 layers, 37,51,73,95,25, tanh and sigmoid output

Opt3 - kerastuner, 6 layers, 6,173,76,146,81,11 tanh and sigmoid output


o	Were you able to achieve the target model performance?

Unfortunately I was not able to reach 75%, the closest was just shy of 73%.


o	What steps did you take in your attempts to increase model performance?

I ran several iterations with different edits.  I changed the amounts of the classification and application_type columns that were allocated to "other".  I also changed the resources that I gave to the model with the amounts of the layers, epochs and the hyperband_iterations.

# Summary 

I came close to the target of 75% accuracy but was not able to meet the benchmark.  Some ideas for increasing that amount given the time and resources would be to change the model/test percentages, try further variations on the input data - especially thinking about the "ask_amt" column to see what changes that would bring.  Always an option to give more resources to the mdoel to learn on as well.
