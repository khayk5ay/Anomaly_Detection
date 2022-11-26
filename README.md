# Anomaly_Detection

This project was inspired by a course i took: Unsupervised Learning, Recommenders, Reinforcement Learning as part of the Machine Learning Specialization offered my DeepLearning.AI and Stanford Online on Coursera

I decided to create my own version of the anomaly detection algorithm using the idea of Gaussian Distribution.

I used numpy and random packages for computing
I used the Matplotlib library for visualisations.

There are 5 methods in the code:

1. generate_dataset
2. get_gaussian_distribution
3. get_probabilities
4. select_threshold

generate_dataset: 
  returns:
    X_train () : Randomly generated values within a specified range that are considered normal
    X_val ()   : Randomly generated values containing values both normal and anomalous
    y_val ()   : Labels for X_val showing the normal values [0] and anomalous values [1]
    

get_gaussian_distribution:
  returns:
    mu () : The mean value(s) of the features in the dataset
    var (): The variance of the features in the dataset
    
get_probabilities:
  returns:
    p_x_j () : An array of the probabilities of each observation
    
select_threshold:
  returns:
    best_F1 () : The F1 Score of the model
    best_epsilon () : The threshold that produced the best F1 Score
    
