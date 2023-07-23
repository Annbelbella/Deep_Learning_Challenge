# Deep_Learning_Challenge
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/6af73166-e70c-4717-8892-192334cfc3ce)


This analysis aims to create a deep learning model using a neural network to predict the success of funding applicants for Alphabet Soup. By training a model on historical data, we aim to classify future applicants into successful or unsuccessful funding categories, assisting Alphabet Soup in making informed decisions.

**Target variable(s):**  The target variable for the model is the "success" or "failure" of funding applicants 

**Feature Variables:** Information about the applicanIt included; classification, application type, affiliation, organization, status etc. 

**Variables removed:** EIN and NAME

I achieved a 73% target model performance which was unfortunaely below the required 75% 

![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/f2695a94-e165-4eea-992b-0827baf54cbb)

### Techniques taken to increase model performance?
1. Increasing the number of neurons and epochs:
By increasing the number of neurons in a layer, the model becomes more expressive and can capture complex patterns in the data.
It also allows the model to refine its predictions and find better parameter values, which can lead to improved accuracy. However, it's important to find a balance as increasing epochs excessively can lead to overfitting. I was only able to achieve 73% .

![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/1ea2f681-5d7b-4278-a5e3-bd3216c4236f)

2. Adding more layers: This can provide the model with additional capacity to capture and represent intricate relationships within the data. Each layer can learn different levels of abstraction, enabling the model to extract more meaningful features and potentially improving accuracy. Deep models with multiple layers have the ability to learn hierarchical representations of the data, which can be advantageous for complex problems.
I was only able to achieve 73%
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/544e7303-7169-4643-be88-64d34fead968)

3. Using a different activation function (tanh for the second layer)

![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/78596aca-b1c1-4d9b-ac9e-74f530c5de71)


 4. Utilizing an Automated Optimiser (such as a hyperparameter tuner):
Automated optimisers, like hyperparameter tuners, systematically explore various combinations of hyperparameters, such as activation functions, number of layers, number of neurons, and epochs. This exploration can help identify the most optimal combination of hyperparameters for your specific problem, potentially leading to higher accuracy. 
Again, I only achieved 73%
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/7b9d6898-18a6-49b1-8133-898f0cea4bb8)


### Conclusion
The deep learning model that I have developed was unable to achieve accuracy higher than 73%. To further improve the model's performance, I would recommend exploring a different algorithm to improve accuracy
and adding more data because increasing the size of the training dataset can help the model learn from a larger and more diverse set of examples.

