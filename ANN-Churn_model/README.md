The given analysis is to check if the customer stays in the bank or leaves the bank. We have used Artificial Neural Network to make the predicition.

The dataset Chrun_Modelling.csv contains 10k data along 14 columns. We have taken following column for the analysis:
    1)CreditScore - credit score of the customer
    2)Geography - the location of the customer - categorical data
    3)Gender - Male/Female - categorical data
    4)Age - Age of the customer
    5)Tenure - years associated with the bank
    6)Balance - Bank balance
    7)NumOfProducts
    8)HasCrCard
    9)IsActiveMember - if the customer is active or not 
    10)EstimatedSalary
    11)Exited (target variable) - target variable to predict if the customer will leave or not.

the dataset is read using pandas and unwanted columns are taken out.
The data preprocessing included Encoding the geography and gender column. The geography is encoded using one-hot encoding method while the Gender column is encoded by label encoder.

Once the data is split into training and testing set, we proceeded with feature scaling method. Feature scaling is an important step in the preprocessing of data for machine learning models. It involves standardizing or normalizing the features in your dataset to ensure they are on a similar scale. We have used standard scalar method for scaling the dataset.

Once the dataset is scaled we proceed with building ANN.
Building ANN involved creating of input layer and 2 hidden layer along with one output layer. This is done using tensorflow and keras. 

Once the ANN is build, we compile and train the model followed by predicting the on test set.

We acheived an accuracy of 85.75% on the test set.
