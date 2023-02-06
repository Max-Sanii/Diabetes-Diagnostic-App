# Diabetes-Diagnostic-App
The objective is to use the dataset from diabetes labs along with experimenting with different Machine Learning algorithms to predict diabetes based on diagnostic measurements.

### Project Description
We can use the historical diagnostic data of the patients who were tested for diabetes in order to calculate the risk of diabetes for other patients who have taken other lab exams that were needed for this prediction.
The app performs diabetes diagnosis based on the patient’s other lab measurements, it allows the technician to choose between three classification algorithms and fine tune its hyperparameters for the best performance. The application uses the models to classify the record either as ‘Diabetes’ or ‘None Diabetes’ depending on the probability value of the prediction, if the probability of diabetes is above 50 %, it labels it as Diabetes in red color, otherwise it shows ‘None Diabetes’ in green color.
The application also shows the performance analytics of the selected model based on its predictions on the test data; these analytics indicate how well the model is trained, and hence how accurate and reliable the prediction is on the sample record. The technician can perform the prediction with different models and choose the prediction result that comes with the best model performance.


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
To run the app, after downloading the files, and we just need to run the below python command, and then the app will be serving in the localhost. (We also need to set the path of the csv file)
Python predict-diabetes-app.py

### Data source:
Original data came from the Biostatistics program at Vanderbilt. This dataset was downloaded from data.world.
The downloaded dataset contains 390 instances (patients) including 60 instances are diabetes and the remaining 330 are not diabetes.
