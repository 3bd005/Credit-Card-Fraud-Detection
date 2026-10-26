# Credit Card Fraud Detection

Detecting credit card fraud with three anomaly detection models: DBSCAN, One-Class SVM and an Autoencoder.

## Project Structure

```
data/        dataset goes here (creditcard.csv)
notebooks/   Fraud_detection.ipynb
reports/     project report (PDF) and presentation (PPTX)
```

## How to Run

1. Download `creditcard.csv` from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and put it in the `data/` folder.
2. Install the libraries:

   ```bash
   pip install pandas numpy pyarrow matplotlib seaborn scikit-learn kneed optuna tensorflow jupyter
   ```

3. Open `notebooks/Fraud_detection.ipynb` and run all cells.

## Results

| Model         | Precision | Recall | F1-Score | ROC-AUC |
|---------------|-----------|--------|----------|---------|
| DBSCAN        | 0.714     | 0.824  | 0.765    | 0.904   |
| One-Class SVM | 0.910     | 0.939  | 0.924    | 0.923   |
| Autoencoder   | 0.785     | 0.705  | 0.743    | 0.946   |
