# Stock Price Prediction with SVM

This project demonstrates a simple stock price movement prediction using a Support Vector Machine (SVM) model in Python. The dataset used is `stock_apple.csv`, and the model predicts whether the stock price will go up or down based on past trading data.

## Prerequisites

Ensure you have the following Python libraries installed:

```bash
pip install pandas scikit-learn
```

## Workflow

1. **Data Preparation**
   - Load stock data from `stock_apple.csv`
   - Define previous day's adjusted close price and volume
   - Compute gain and classify the movement as `Up` (1) or `Down` (0)
   - Handle missing values

2. **Feature Engineering**
   - Create `volume_ratio` (current volume / previous volume)
   - Create `close_price_ratio` (current adjusted close price / previous adjusted close price)
   - Shift target labels to align with prediction inputs
   
3. **Model Training and Evaluation**
   - Split data into training and test sets (80%-20%)
   - Normalize features using `StandardScaler`
   - Train an SVM model with the RBF kernel
   - Evaluate performance using accuracy score and confusion matrix

## Usage

Run the Jupyter Notebook in an environment where you have the necessary dependencies installed. The script will output the model's accuracy and confusion matrix.

## Output Example

```
number of correct samples: 45
accuracy: 0.75
confusion matrix:
[[30 10]
 [ 5 20]]
```

## Notes
- The dataset must be structured correctly with columns such as `Adj Close` and `Volume`.
- Ensure there are no missing values before training.
- Adjustments to features or hyperparameters may improve model performance.

