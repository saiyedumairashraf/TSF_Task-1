# TSF_Task-1 : THE SPARKS FOUNDATION :Prediction using Supervised ML-LinearRegression
This code is a Python script that demonstrates the use of linear regression to predict the percentage score of a student based on the number of hours they study. Here's a breakdown of what the code does:

Importing necessary libraries: This code imports the required libraries for data manipulation (pandas), numerical operations (numpy), data visualization (matplotlib.pyplot), and the linear regression model (LinearRegression from sklearn.linear_model).

Reading the data: The code reads the data from a provided URL using pd.read_csv() function from the pandas library. The data is assumed to be in CSV format.

Splitting the data: The code splits the data into input (X) and output (y) variables. The input variable X contains all columns except the last one, and the output variable y contains the last column. This assumes that the input data has a specific structure, where the first column represents the number of hours studied and the second column represents the percentage score.

Splitting the data into training and testing sets: The code uses train_test_split() function from sklearn.model_selection to split the data into training and testing sets. It assigns 80% of the data to training (X_train and y_train) and 20% of the data to testing (X_test and y_test).

Creating and fitting the linear regression model: The code creates an instance of the LinearRegression model. It then fits the model to the training data using the fit() method, which finds the best-fit line based on the given input and output variables.

Predicting the percentage of a student who studies for 9.25 hrs/day: The code creates a variable hours containing the number of hours a student studies ([[9.25]]). It uses the trained model to predict the percentage score for this input using the predict() method and stores it in the variable predicted_score.

Printing the predicted score: The code prints the predicted score for 9.25 hours of study using the print() function. It formats the output to display the predicted score with two decimal places.

The output of running this code would be: Predicted Score for 9.25 hours of study: 91.40%, indicating that the model predicts a score of 91.40% for a student who studies for 9.25 hours per day.

Releases
