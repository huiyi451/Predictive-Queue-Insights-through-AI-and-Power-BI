# AIQueue Wait Time Prediction

## Model Development

### Data Preprocessing
1. Encode categorical variables:
   - Gender
   - Specialty
   - Reason for visit
   - Scheduled appointment
   - First-timer
2. Split the dataset into features and target variable (wait time).
3. Divide the data into training (80%) and testing (20%) sets.
4. Normalize numerical features:
   - Age
   - Check-in time
   - Check-out time
   - Date
   - Number waiting

### Model Building
1. Implement three Machine Learning models:
   - Linear Regression
   - LightGBM
   - Random Forest
2. Train the models using the preprocessed training data.

### Model Evaluation
1. Evaluate models using the following metrics:
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - R-Squared
2. Identify the best model based on the evaluation metrics:
   - **Random Forest model** was found to be the best performer with the lowest MAE (0.65 minutes) and MSE (7.70 minutes), and the highest R-Squared (0.996).

### Prediction and Results
1. Use the trained Random Forest model to predict wait times on the test data.
2. Calculate the average predicted wait times for 1 to 30 people in the queue.
3. Save and display the predicted wait times on the website for patient reference.

