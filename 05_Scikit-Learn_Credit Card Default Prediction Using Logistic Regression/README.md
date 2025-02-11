# Credit Card Default Prediction Using Logistic Regression

## Objective

This project aims to predict whether credit card users will default using the Logistic Regression model. The dataset comes from default_credit_card.csv, and the data is split into training and testing sets for model training and prediction.

## Installation Requirements

To run this project successfully, you need to install the following Python packages:

pip install pandas numpy scikit-learn

## File Structure

default_credit_card.csv: The dataset file containing user information and their default labels.

Credit_Card_Default_Prediction.ipynb: The Jupyter Notebook containing the logistic regression training and prediction process.

## Project Steps

1. **Read the Dataset**

The dataset is loaded using pandas, and the first few rows are displayed to understand the structure of the data.

2. **Set the Feature Matrix and Target Labels**

The feature matrix (X) is created by excluding the target column Y, and the target (y) is set as the Y column which indicates whether the user defaulted.

3. **Split the Data**

The dataset is split into a training set (70%) and a testing set (30%) using train_test_split.

4. **Standardize the Features**

The features are standardized using StandardScaler to ensure that all features are on the same scale, which helps improve the model’s performance.

5. **Train the Logistic Regression Model**

The logistic regression model is trained using the training set. The model is then used to predict outcomes on the testing set.

6. **Evaluate the Results**

The accuracy of the model is evaluated using accuracy_score, which compares the predicted values with the actual outcomes from the testing set. The number of correct predictions is also displayed.

## Jupyter Notebook Usage

Open Jupyter Notebook and ensure your default_credit_card.csv file is in the same directory as the notebook.

Run the cells in the notebook to load the dataset, process the data, train the model, and evaluate its performance.

## Results

Once the notebook is run, the number of correct predictions and the accuracy of the model will be displayed as output.

## Notes

Ensure that the default_credit_card.csv file is correctly formatted and located in the appropriate directory.

If the dataset contains missing values or anomalies, you may need to clean the data before running the model.