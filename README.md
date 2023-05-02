# Reinforcement-Learning-offline-learning-vs-imitation-Learning
The purpose of this expriment is to compare the performance of offline fitted q learning with imitation learning using logistic Regression on data generated
in the following three scenarios for the cartpole-v1 enviroment in gymnasium: 

1. Data generated by expert policy
2. Data generated by random policy 
3. Data with half of them generated by expert policy and half of them with the random policy. 

The Expert policy is an vanilla implementation of actor critic method first trained with 700 episodes. For each scenarios 500 episode worth of data is 
generated and for each dataset we create 3 sub-datasets each with length 100,250, and 500. The average rewar of of each subdataset is listed below:

Random Averages:

 100: 22.29 
 
 250: 21.44 
 
 500: 21.96
 
Expert Averages:

 100: 154.96 
 
 250: 146.732 
 
 500: 147.64
 
Half-Half Averages:

 100: 80.24 
 
 250: 82.324 
 
 500: 84.454
 
 Then using the fitted q-learning and imitation learning to learn from the above 9 datasets obtain us the final result of our expriment. 
 
