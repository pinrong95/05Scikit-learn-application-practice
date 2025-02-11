# Titanic Survival Prediction (Naive Bayes)

This project uses the Titanic dataset and the Naive Bayes classifier to predict whether passengers survived or not.

## Dataset

The dataset is from the Kaggle Titanic competition: [Titanic Dataset](https://www.kaggle.com/c/titanic/data).

## Requirements

You need to install the following Python packages:
- pandas
- numpy
- matplotlib
- scikit-learn

To install dependencies, run:
```
pip install -r requirements.txt
```

## Process

1. **Load Dataset**: The Titanic dataset is loaded using `pandas.read_csv()`.
2. **Preprocessing**:
   - Encode the `Sex` and `Embarked` columns.
   - Drop rows with missing values.
3. **Features and Target Variable**:
   - Features include `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, and `Embarked`.
   - Target variable is `Survived`.
4. **Train-Test Split**: Split the data into training and test sets.
5. **Model Training**: Train a Naive Bayes model on the training data.
6. **Prediction**: Use the trained model to predict survival on the test data.
7. **Evaluation**: Evaluate the model using accuracy and confusion matrix.

## License

This project is licensed under the MIT License.
```

This version is short and clear, covering the key points of the project.