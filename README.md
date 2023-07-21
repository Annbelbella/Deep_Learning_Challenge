# Deep_Learning_Challenge
![image](https://github.com/Annbelbella/Deep_Learning_Challenge/assets/124645643/6af73166-e70c-4717-8892-192334cfc3ce)


This analysis aims to create a deep learning model using a neural network to predict the success of funding applicants for Alphabet Soup. By training a model on historical data, we aim to classify future applicants into successful or unsuccessful funding categories, assisting Alphabet Soup in making informed decisions.

Target variable(s): The target variable for the model is the "success" or "failure" of funding applicants 

Feature Variables: Information about the applicanIt included; classification, application type, affiliation, organization, status etc. 

Variables removed: EIN and NAME

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
The deep learning model that I have developed was unable to achieve accuracy higher than 73%. To further improve the model's performance, I would recommend exploring a different algorithm to improve accuracy
and adding more data because increasing the size of the training dataset can help the model learn from a larger and more diverse set of examples.

....................................................................................................................................................................................................................................................................................................

## Project Instructions
### Step 1: Preprocess the Data
Using your knowledge of Pandas and scikit-learn’s StandardScaler(), you’ll need to preprocess the dataset. This step prepares you for Step 2, where you'll compile, train, and evaluate the neural network model.

Start by uploading the starter file to Google Colab, then using the information we provided in the Challenge files, follow the instructions to complete the preprocessing steps.

Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
What variable(s) are the target(s) for your model?
What variable(s) are the feature(s) for your model?
Drop the EIN and NAME columns.

Determine the number of unique values for each column.

For columns that have more than 10 unique values, determine the number of data points for each unique value.

Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

Use pd.get_dummies() to encode categorical variables.

Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.

Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

### Step 2: Compile, Train, and Evaluate the Model
Using your knowledge of TensorFlow, you’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. You’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once you’ve completed that step, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.

Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

Create the first hidden layer and choose an appropriate activation function.

If necessary, add a second hidden layer with an appropriate activation function.

Create an output layer with an appropriate activation function.

Check the structure of the model.

Compile and train the model.

Create a callback that saves the model's weights every five epochs.

Evaluate the model using the test data to determine the loss and accuracy.

Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity.h5.

### Step 3: Optimize the Model
Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

Use any or all of the following methods to optimize your model:

Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
Dropping more or fewer columns.
Creating more bins for rare occurrences in columns.
Increasing or decreasing the number of values for each bin.
Add more neurons to a hidden layer.
Add more hidden layers.
Use different activation functions for the hidden layers.
Add or reduce the number of epochs to the training regimen.

Note: If you make at least three attempts at optimizing your model, you will not lose points if your model does not achieve target performance.

Create a new Google Colab file and name it AlphabetSoupCharity_Optimization.ipynb.

Import your dependencies and read in the charity_data.csv to a Pandas DataFrame.

Preprocess the dataset as you did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.

Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.

Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.
