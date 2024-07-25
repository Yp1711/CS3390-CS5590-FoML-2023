# Meal Duration Estimator

## Overview

This project aims to predict the time it takes to finish food in the mess, considering various factors such as day, time, holiday, and meal category. Linear regression may not be suitable for this problem due to the nature of the output.

## Data Collection

The data was collected over a period of 2 weeks, recording the time taken to finish food for different meals (breakfast, lunch, tea, dinner). Features include day of the week, time of day, whether it's a holiday, and the meal category.

## Model Selection

After considering the nature of the problem, a mixture of weighted meand and polynomial regression model was chosen for its ability to capture complex relationships and interactions between features.

## Running the Code

1. **Dependencies**:
   - Ensure you have the necessary Python libraries installed. You can do this using the following command:
     ```
     pip install [Module]
     ```
1. **Exploratory Data Analysis**:
    - Some features like 'Special_dinner' & 'Holiday' looked usless based on the their plots. so removed such features. Other task under this phase includes:-
      - Renaming Colums
      - Droping irrelavent columns
      - Droping missing/null Values
      - Plotting Charts to investigate relationship between features and target variable. 
      - Detecting Outliners if any

3. **Training the Model**:
   - Analyzing the feature matrix and target vector on per feature vs target vector basis, we got to know that the categorical features 'Category' and 'Day' clusters around their emperical mean with respect to the target vector. And Numerical feature 'Start' follows polynomial regression with polynomial of degree 3. So we basically came up with a fit to the data that will take a weighted averages of the mean of categorical data and predicted value of the numerical data. So build a model in that way and trained it using 80% of the dataset.

4. **Testing the model**:
    - We tested the performance of the model on later 20% of the data. It showed up a R-Square value of ~0.86, indicating model's prediction performance of 86%. 

5. **Comparison Output**:
   - The comparison with Linear Regression based on R-Square Score showed the results like:-
   ```
   Linear Regression Performance: 0.55
   Our Model Performance: 0.86
   ```
## Comments in Code

The code is extensively commented to provide context and explanations for each step. Please refer to the comments for a detailed understanding of the code.
