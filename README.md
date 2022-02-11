# Neural_Network_Charity_Anlayisis

## Overview

The present project tries to determine a model to predict the success of charities, based on variables provided by the cliente.

## Results

### Original data

![original](https://user-images.githubusercontent.com/89816213/153541724-68bfaead-5658-42a0-8968-b3fc5537dba6.PNG)

The original data contains information both useful and unnecessary, therefore we must start removing the unnecessary data.

#### Drop-values

![drop EIN_Name](https://user-images.githubusercontent.com/89816213/153541687-8b8316df-90cb-4f36-bb46-1fb11629676c.PNG)

The first data to be removed is the name and id code of each charity, since this two variables are most likely not a factor in determining wether a charity will or not be successful.

### Data Preprocessing

![type_count](https://user-images.githubusercontent.com/89816213/153542321-f4d604aa-ff30-4b47-a2ed-0e1a4a7fc488.png)

![classification](https://user-images.githubusercontent.com/89816213/153541953-f774eec9-ef28-420c-bb87-183fbeb318b8.png)

The previous images show how we determine which data to consider for our analysis given a certain distribution, we consider all data under a certain range to diminish outliers. 

#### Target and Variables

![target](https://user-images.githubusercontent.com/89816213/153541530-4818b5bc-a686-4c42-a241-ee2e73e802c2.PNG)

Once we have cleansed our data we have to determine which factor is our target. Here it's quite simple, since we are trying to determine the probability of  a charity to succeed, our target is the IS_SUCCESSFUL column.

### Compiling, Training and Evaluating the Model
![Neurons_layers_epochs](https://user-images.githubusercontent.com/89816213/153541960-1ec24298-58f0-4533-ae10-fb65967cf6ca.PNG)
![original](https://user-images.githubusercontent.com/89816213/153541973-395a0fd5-13d5-4878-92d0-253f897f3c42.PNG)
![original_acc](https://user-images.githubusercontent.com/89816213/153541987-63ce2cf7-f75b-46c4-b6d6-0a345ad344a6.PNG)

In the previous images we can see the process to scale, train and test our model, as well as the result. This result can be considered low by certain criteria, though it's already more succesful than guessing.

### Optimizing the Model

![optim](https://user-images.githubusercontent.com/89816213/153542052-79926e8f-8fb3-4580-9da4-273016356b6c.PNG)

Trying to reach a higher accuracy (75%) this model has been changed in the following ways:
- Adding a hidden layer
- Changing the number of neurons
- Increasing the number of epochs

![optim_acc](https://user-images.githubusercontent.com/89816213/153542061-d0d68365-bcad-4f92-b763-ea11fba90f05.PNG)

The result does not show any improvement over the previous model, which might lead us to think that this particular dataset might contain some information that creates "noise" in our model.
