# Module 21 Deep Learning Challenge - Alphabet Soup Analysis Report 

 ![AI-artificial-intelligence-brain-deep-learning](https://github.com/CBURKHARDT47/deep-learning-challenge/assets/128064003/7b908228-7830-42ca-a7ce-d4af0deff47c)


## 1. Overview of the Analysis
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## 2. Results

### Data Preprocessing
I read in the charity_data.csv to a Pandas DataFrame from the URL provided in the Jupyter Notebook file opened through Google Colab. Using my knowledge of Pandas and scikit-learn’s StandardScaler(), I preprocessed the dataset. 

*What variable(s) should be removed from the input data because they are neither targets nor features?
The first step in the data processing was to drop the EIN and NAME columns because they do not provide any relevant data to the objective of the analysis and removing unnecessary data helps optimize the model.

*What variable(s) are the features for your model?
Any remaining columns were considered as features for our model. 

*What variable(s) are the target(s) for your model? 
The "IS_SUCCESSFUL" variable was the target for my model. A value of '1' meant the funding loan was utilized successfully/effectively, and a value of '0' meant the funding was unsuccessful/ineffective. 

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
There were 3 layers in total after applying the neutral networks. The number of hidden nodes in the hidden layer is typically determined based on various factors, including the number of features in your dataset and your specific problem. There is no strict rule that the number of hidden nodes should be equal to the number of features, but it's a common approach so I went with that approach. 
![image](https://github.com/CBURKHARDT47/deep-learning-challenge/assets/128064003/6ac13979-5a28-4a88-b8eb-0dd48b4a6768)


There were 477 parameters created by the 3 layers in the training model. 
![image](https://github.com/CBURKHARDT47/deep-learning-challenge/assets/128064003/21238164-cb8d-4d4b-b2e7-e1f718155a83)


Were you able to achieve the target model performance?
The first attempt was about 73% accurate but we were aiming for at least 75% accuracy. 
![image](https://github.com/CBURKHARDT47/deep-learning-challenge/assets/128064003/9957a9f7-69a2-40df-9e3c-fdc752a79a72)


What steps did you take in your attempts to increase model performance?
I attempted to optimize the model during the second attempt using the "NAME" column and this increased the accuracy from 73% to 79% with 3,298 parameters.
![image](https://github.com/CBURKHARDT47/deep-learning-challenge/assets/128064003/d293bd26-7f74-4561-8c21-bde94cc561a3)

Multiple layers should be used as this helps to train the machine learning model based on filtering the data through the multiple layers. 
![image](https://github.com/CBURKHARDT47/deep-learning-challenge/assets/128064003/c3dfe264-cd6b-4aa3-acc0-0e2de2fe3a1b)


### 3. Summary

