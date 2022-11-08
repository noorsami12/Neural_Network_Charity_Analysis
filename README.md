# Neural_Network_Charity_Analysis

## Overview of the Analysis

For the purpose of this assignment, I used machine learning and neural networks to create a binary classifier capable of predicting whether investment applicants will be successful if funded by the foundation Alphabet Soup. Using a csv dataset that contains metadata about over 34,000 organizations funded by Alphabet Soup, I pre-processed the data in order to compile, train, and evaluate the neural network model. Then I optimized the model to obtain peak accuracy by making various tweaks such as adding additional neurons in hidden layers and changing the number of training epochs. 

## Results

#### Data Preprocessing
- For my model, the target variable is the “is_successful” column which determines whether or not the investment was successful or not based on binary values. 
- The variables that are the features for the model are the length of the scaled data. 
- There are no variables that could be removed from the data. 

#### Compiling, Training, and Evaluating the Model
- I selected 10 nodes for hidden layer 1 and 5 nodes for hidden layer 2 to start with. I included two hidden layers and an output layer. However, this gave me an accuracy below 75% so I decided to optimize the model by increasing the number of nodes. I changed layer 1’s nodes to 50 and layer 2’s nodes to 25. I kept the same number of layers. This was much more successful. 
- I was able to achieve the target model performance on the third try through a combination of changing the number of neurons in the layers and changing the number of training epochs. The ideal numbers were 50 and 25 for hidden layers 1 and 2 respectively and 75 epochs. This gave me an accuracy of 76%. 
- The steps I took to change the model performance were first to change the parameters of replacement values when first cleaning the data. This did not make much of a difference. I then changed the number of training epochs to 150, which did not help. I finally changed epochs to 75 and changed the number of neurons in each hidden layer and was able to achieve the target. 

![target_accuracy](https://github.com/noorsami12/Neural_Network_Charity_Analysis/blob/608cb182ff96019ce6b3dcaa63d8e08540bca481/target_accuracy.png)


## Summary

Overall, my deep learning model was able to achieve 76% accuracy with 85% loss. Another effective model to investigate the success of investments would be using a confusion matrix. A confusion matrix would show us a breakdown of predictions on whether to invest or not. We could derive various statistical measures from the matrix, such as accuracy, precision, sensitivity, and specificity. It would also be helpful to see the misclassification rate and the null error rate so we could accurately determine the effectiveness of our model. 
