21. deep-learning-challenge
Charity Funding Predictor
Overview

The goal of this project is to create an algorithm using machine learning and neural networks to predict whether applicants will be successful if funded by the fictional non-profit foundation, Alphabet Soup.
Process

I was given a CSV file that I read into Pandas. This file contained a number of organizations that have received funding from the fictional foundation along with several columns of metadata about each organization.

PREPROCESSING

I preprocessed the data as follows

 - Dropping non-beneficial columns.

 - Finding the number of data points for each unique value for each of the columns that had more than 10 unique values.
 
 - Choosing a cutoff point.
 
 - Used pd.get_dummies() to convert categorical data to numeric.

 - Divided the data into a target array and feature arrays. 

 - Applied the train_test_split to create a testing and a training dataset.

 - Used StandardScaler to scale the training and testing sets.


COMPILING, TRAINING, AND EVALUATING THE MODEL

The model was required to achieve a target predictive accuracy higher than 75%. I made two attempts and each model landed at the 73% mark

Results from each model attempt are detailed below:

ATTEMPT 1

The first attempt (h5_files/AlphabetSoupCharity1.h5) resulted in an accuracy score of 73.80% This was the highest accuracy score of the three models. This means that 73.80% of the model’s predicted values align with the dataset’s true values.


ATTEMPT 2
My second attempt (h5_files/AlphabetSoupCharity_optimization_1.h5) resulted in an accuracy score of 73.48%. This means that 73.48% of the model’s predicted values align with the dataset’s true values. Which was worse than the first model.


ATTEMPT 3
My Third attempt (h5_files/AlphabetSoupCharity_optimization_2.h5) was unfortunately unfinished as I ran out of time to get the model working accurately - as seen in the notebook I was having a error with my neural network that I could not solve.


In summary unfortunately I ran out of time to further optimize the the algorithm to get a more accurate score in my third attempt - the scores were never higher than the previous two attempts. The first attempt using a basic neural network had the highest accuracy where as I feel Keratuner would have needed more cleaning / binning of data to get a more accurate final reading. So to finialize the basic build of the model actually turned out to be the most accurate. Which is interesting as it points out that less can actually be better than more complex iterations.

