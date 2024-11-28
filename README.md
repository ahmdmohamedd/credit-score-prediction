# Credit Score Prediction

This project implements a neural network-based system for predicting credit scores using the UCI Credit Card Default dataset. The model evaluates the likelihood of a credit card holder defaulting on their payments, achieving an accuracy of 82%.

---

## Features

- **Neural Network Architecture**: 
  - Built using TensorFlow/Keras with two hidden layers and dropout for regularization.
- **Data Preprocessing**: 
  - Standardized features and one-hot encoded target variable.
- **Model Evaluation**: 
  - Detailed performance metrics including precision, recall, F1-score, and support.
- **Visualization**: 
  - Training and validation accuracy trends plotted for better understanding of model performance.

---

## Dataset

The [UCI Credit Card Default Dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) contains payment data of credit card clients from Taiwan.  
- **Features**: Includes demographic information, payment history, and billing statements.  
- **Target**: Binary classification indicating whether the client defaulted on payments (`0` = No, `1` = Yes).

---

## Performance Summary

The model evaluation results are as follows:

| Metric      | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| **Class 0** | 0.83      | 0.96   | 0.89     | 4687    |
| **Class 1** | 0.68      | 0.31   | 0.42     | 1313    |
| **Overall Accuracy** | 82% | | | 6000 |

- Class 0 (No Default): The model performs well with high precision and recall.  
- Class 1 (Default): The model underperforms in predicting defaults, which may be improved using techniques like oversampling or class weighting.

---

## Dependencies

The project uses the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `tensorflow`

Install the dependencies using:
```bash
pip install pandas numpy scikit-learn matplotlib tensorflow
```

---

## Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/ahmdmohamedd/credit-score-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd credit-score-prediction
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook credit_score_prediction.ipynb
   ```

---

## Project Structure

- `credit_score_prediction.ipynb`: Contains the entire implementation, from data preprocessing to model evaluation.
- `README.md`: Project documentation.

---

## Future Enhancements

To improve the system, the following could be implemented:
- **Addressing Class Imbalance**: Use techniques like SMOTE or class weighting to improve recall for Class 1 (defaults).
- **Feature Engineering**: Analyze feature importance and explore derived features.
- **Hyperparameter Optimization**: Tune model architecture and training parameters for better performance.


--- 
