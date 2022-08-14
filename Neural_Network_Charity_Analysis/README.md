# Neural_Network_Charity_Analysis

# Overview

    With the use of Machine Learning and Neural Networks as well as the available dataset, a binary classifer was created that will help predict if 
    the applicants that were to be funded by the Alphabet Soup charity would be successful. The dataset that was used contains various measures on 34,000
    orginizations that have been fully funded by the Alphabet Soup Charity. Furthermore, this project was comprised of the following steps:
        
        -Processing the data for a Neural Network
        -Compilie, Train and Evaluate the Model
        -Optimizing the Model
        
 # Results
  # Data Preprocessing
      -The IS_SUCESSFUL Coloumn was used as a target for my model
      -All the coloumns except IS_SUCCESSFUL were considered features and were ultimately the ones that I dropped
      -Variables that were neither targets or features and ended up being dropped were: EIN and NAME because they had little to no impact with reguards to the
      outcome.
      
  # Compiling, Training and Evaluating the Model
    
    -For my neural network there were 2 hidden layers. My first layer had 80 neurons, the second has 30 there is also an output layer. The first and second hidden layer
    have the "relu" activation function and the activation function for the output layer is "sigmoid."
    
    ![image](https://user-images.githubusercontent.com/101299252/184558252-a3ee54d3-b0b5-4c96-893b-d0d02dd41015.png)

   -The model was not able to reach the target of 75% due to an accuracy of 69%.
    
   ![image](https://user-images.githubusercontent.com/101299252/184558301-8145d0ca-0b41-4665-a092-a81cde3087f7.png)

   # Steps taken to improve model preformance
   
    -Remeoved an additional feature, the "USE_CASE" coloumn, however it resulted in a lower accuracy model of 63%.

    ![image](https://user-images.githubusercontent.com/101299252/184558365-696342d2-a46b-47ef-b3b5-d38e769adf25.png)

    ![image](https://user-images.githubusercontent.com/101299252/184558357-6341a071-95e7-470f-b8fb-ab9fc55655a0.png)
  
    - Added additional neurons to the hidden layers while also adding hidden layers. This lowered the accuracy of 53%.
    
    ![image](https://user-images.githubusercontent.com/101299252/184558451-fad4e22d-293e-4f98-bc90-d695aab3df30.png)

    ![image](https://user-images.githubusercontent.com/101299252/184558456-5bb1ecf8-4dab-44bd-8aba-2c378ae39228.png)

    -Changing activation function of output layer from "sigmoid" to "tanh". This brought the model down again to 50%
    
    ![image](https://user-images.githubusercontent.com/101299252/184558499-64931d3c-9d73-4383-a3e9-4d240242e70a.png)

   ![image](https://user-images.githubusercontent.com/101299252/184558507-1c89f9b8-e873-4448-a50a-2777af0593ea.png)

  # Summary
  
    After taking steps to optimize the model the accuracy score resulted in 50% form an inital neural score of 69%. This difference can be related to the model 
    being overfitted. Further steps to optimize the model can be removing more features or to add more data into the dataset. Due to the low accuracy score, 
    random forest classifiers could have been an option due to their sufficent number of estimators the program has which can result in better accuracy. Furthermore,
    these models have a faster preformance than neural networks and helps avoid the data from running into the same overfitting issue. 
