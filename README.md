# deep_learning_challenge
In this project, I use machine learning and neural network algorithms to create a binary classifier that can predict weather an applicant if funded by an foundation will be successful or not. I use csv data file which provides different features of more than 30,000 organizations previously funded by the foundation. 

<br>

First, we preprocess the data by removing not important columns as well as using binning to group the rare data values together. We also convert the categorical data values to numerical using get_dummies function in pandas. The dataframe was splitted into target and the features columns where the organization's success/failure was the target column. The data was then splitted into train and test dataset using scikit learn train_test_spilit module. Teh train data was then scaled using scalar transform using Standardscalar module from sk-learn. The scaling was then applied to transform train and test data. 

<br>

After the data preprocessing, I created a deep learning neural network model to from tensor-flow module to to train a neural network on the preprocessed train data. I started from two hidden layers with ~10 neurons in each and later increased the number of neurons to see if hte performance of the model changes. Even with changing number of nodes, activation function, as well as number of hidden layers, the accuracy stayed around 73%, with training loss around 0.5 to 0.6. 
