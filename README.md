# Deep_Learning_Challenge
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, i used the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/6af73166-e70c-4717-8892-192334cfc3ce)


I achieved a 73% target model performance which was unfortunaely below the required 75% 

![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/9d64e543-01ed-4e05-bb93-a155027487b9)

### Techniques taken to increase model performance?
1. Increasing the number of neurons and epochs:
By increasing the number of neurons in a layer, the model becomes more expressive and can capture complex patterns in the data. This allows for better representation of the underlying relationships between the features and the target variable, potentially leading to higher accuracy.
Increasing the number of epochs gives the model more opportunities to learn from the data and adjust the weights. It allows the model to refine its predictions and find better parameter values, which can lead to improved accuracy. However, it's important to find a balance as increasing epochs excessively can lead to overfitting. I was only able to achieve 73% .

![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/1ea2f681-5d7b-4278-a5e3-bd3216c4236f)


2. Adding more layers: This can provide the model with additional capacity to capture and represent intricate relationships within the data. Each layer can learn different levels of abstraction, enabling the model to extract more meaningful features and potentially improving accuracy. Deep models with multiple layers have the ability to learn hierarchical representations of the data, which can be advantageous for complex problems.
I was only able to achieve 73%
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/544e7303-7169-4643-be88-64d34fead968)

3. Using a different activation function (tanh for the second layer):
Introducing a different activation function, such as tanh, can affect how the model interprets and transforms the inputs. Different activation functions have different properties and can capture different types of non-linearities. By using tanh, it introduces a different non-linearity that may better suit the problem at hand, potentially leading to increased accuracy.
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/b0eabaec-5713-4dd0-8c56-49e03bc979a1)


 5. Utilizing an Automated Optimiser (such as a hyperparameter tuner):
Automated optimisers, like hyperparameter tuners, systematically explore various combinations of hyperparameters, such as activation functions, number of layers, number of neurons, and epochs. This exploration can help identify the most optimal combination of hyperparameters for your specific problem, potentially leading to higher accuracy. It saves you from manually trying out different combinations and allows the optimiser to leverage its search algorithms to find the best configuration.
Again, I was only able to achieve 73%
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/58f21ef8-278c-4660-b576-ea1358b15f99)

### Conclusion
The deep learning model that I have developed was unable to achieve accuracy higher than 73%. To further improve the model's performance, I can consider;
- Adding more data because increasing the size of the training dataset can help the model learn from a larger and more diverse set of examples.
- Trying a different algorithm, such as Random Forest to allow focusing on the most informative features and potentially improve accuracy.

