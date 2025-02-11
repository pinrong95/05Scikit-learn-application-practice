# Pima Indians Diabetes Prediction Using Logistic Regression

## Objective

This project aims to predict whether a person has diabetes based on four features (`pregnant`, `insulin`, `bmi`, `age`) using the `Logistic Regression` model. The dataset comes from `pima-indians-diabetes.csv`, and the data is split into training and testing sets to evaluate the model's performance.

## Installation Requirements

To run this project successfully, you need to install the following Python packages:

```bash
pip install pandas numpy scikit-learn
```

## File Structure

- `pima-indians-diabetes.csv`: The dataset file containing medical data and labels indicating whether the person has diabetes.
- `Diabetes_Prediction.ipynb`: The Jupyter Notebook containing the logistic regression model training and evaluation process.

## Project Steps

### 1. Load the Dataset

The dataset `pima-indians-diabetes.csv` is loaded using `pandas`. The first few rows are displayed to understand the structure of the data.

### 2. Set the Feature Matrix and Target Labels

The feature matrix (`x`) is created by selecting four relevant variables: `pregnant`, `insulin`, `bmi`, and `age`. The target (`y`) is the `label` column, which indicates whether the person has diabetes (1) or not (0).

### 3. Split the Data

The dataset is split into a training set (70%) and a testing set (30%) using `train_test_split` with `random_state=1` for reproducibility.

### 4. Standardize the Features

Both the training and testing sets are standardized using `StandardScaler`. This ensures that all features are on the same scale, which helps improve model performance.

### 5. Train the Logistic Regression Model

The logistic regression model is trained on the standardized training data. The model is then used to predict the labels for the testing set.

### 6. Evaluate the Model

The accuracy of the model is calculated by comparing the predicted labels with the actual labels from the testing set using `accuracy_score`. The number of correct predictions is also displayed.

## Jupyter Notebook Usage

1. Open Jupyter Notebook and ensure that the `pima-indians-diabetes.csv` file is in the same directory as the notebook.
2. Run the notebook cells to load the dataset, process the data, train the logistic regression model, and evaluate its accuracy.

## Results

Once the notebook is run, the number of correct predictions and the model's accuracy will be displayed.

## Notes

- Make sure the `pima-indians-diabetes.csv` file is correctly formatted and located in the appropriate directory.
- If the dataset contains missing values or anomalies, it may require additional preprocessing steps before running the model.

---

This README provides an overview of your Jupyter Notebook, describing the key steps, requirements, and instructions for use. Let me know if you'd like to adjust or add anything!