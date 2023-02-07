# Diabetes-Diagnostic-App
The objective is to use the dataset from diabetes labs to train a Machine Learning model to predict diabetes based on diagnostic measurements. The app allows you to pick between six different algorithms as your classifier model; in addition, it can find the algorithm with the best performance for your data.

### Project Description
We can use the historical diagnostic data of the patients who were tested for diabetes in order to calculate the risk of diabetes for other patients who have taken other lab exams that were needed for this prediction.
The app performs diabetes diagnosis based on the patient’s other lab measurements, it allows the technician to choose between three classification algorithms and fine tune its hyperparameters for the best performance. The application uses the models to classify the record either as ‘Diabetes’ or ‘None Diabetes’ depending on the probability value of the prediction, if the probability of diabetes is above 50 %, it labels it as Diabetes in red color, otherwise it shows ‘None Diabetes’ in green color.
The application also shows the performance analytics of the selected model based on its predictions on the test data; these analytics indicate how well the model is trained, and hence how accurate and reliable the prediction is on the sample record. The technician can perform the prediction with different models and choose the prediction result that comes with the best model performance.

### Application 
The Application consists of three sections:

#### Select Classifier and Train the model
The top section allows the user to select a model, pick the number of training data and click on Train button, then the model starts training, and shows the best hyperparameter values computed by the Grid search algorithm:
![image](https://user-images.githubusercontent.com/118564295/217125220-a5996ec4-c962-4408-8990-1661ab75a5f5.png)

#### Predict
This section shows a sample record that was randomly picked from the dataset, the user can edit the values or enter a new input, and then click on the Predict button, and then the trained model will perform the classification on this test data:
![image](https://user-images.githubusercontent.com/118564295/217125285-24d1b39a-fe70-4c97-871e-f03a5efe09e2.png)

#### Model Performance
The bottom section corresponds to the performance of the trained model, the first panel shows three performance scores, which are calculated based on the predictions on the test data. The confusion matrix is also provided, which upon hovering on each box, shows the count of true or false predictions on the test data. The pie chart on the right shows the same data in percentage, so the user can see the fractions of the prediction results.
![image](https://user-images.githubusercontent.com/118564295/217125338-e0f04f2e-ad17-42ac-8ad1-f0c693b9f71a.png)


### Methods Used
Machine Learning
Logistic Regression
KNN
Naive Bayes
Decision Tree
Random Forest
Gradient Boosting

### Technologies
Python
Dash
Numpy
Scikit-learn
Pandas
Matplotlib

### Instructions:
The application is created by Dash framework in python, the file “predict-diabetes-app.py” contains the whole code including both the logic and the layout of the app. 
To run the app, first download the files, and we just need to run the below python command, and then the app will be serving in the localhost. (We also need to set the path of the csv file)
Python predict-diabetes-app.py

### Data source:
Original data came from the Biostatistics program at Vanderbilt. This dataset was downloaded from data.world.
The downloaded dataset contains 390 instances (patients) including 60 instances are diabetes and the remaining 330 are not diabetes.
