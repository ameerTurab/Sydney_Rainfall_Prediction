#Project Workflow

```text
Historical Weather Data
           │
           ▼
   Data Preprocessing
           │
           ▼
 Exploratory Data Analysis
           │
           ▼
 Feature Engineering
           │
           ▼
 ┌─────────────────────┐
 │ Dense Neural Network│
 └─────────────────────┘
           │
           ▼
 ┌─────────────────────┐
 │        LSTM         │
 └─────────────────────┘
           │
           ▼
 Model Evaluation
           │
           ▼
 Performance Comparison
```
# Deep Learning Models

## Dense Neural Network (DNN)

The Dense Neural Network (DNN) is a feed-forward neural network designed to classify whether a day is rainy based on meteorological variables. The model consists of fully connected layers with dropout regularization to reduce overfitting.

### Model Architecture

![Dense Model Architecture](images/dense_model_architecture.png)

### Training Performance

Training Accuracy

![Dense Accuracy](images/dense_training_accuracy.png)

Training Loss

![Dense Loss](images/dense_training_loss.png)

### Model Evaluation

Confusion Matrix

![Dense Confusion Matrix](images/dense_confusion_matrix.png)

---

## Long Short-Term Memory (LSTM)

The Long Short-Term Memory (LSTM) network captures temporal dependencies within weather observations by learning from sequences of previous days. This architecture is particularly suitable for rainfall forecasting because weather patterns evolve over time.

### Model Architecture

![LSTM Model Architecture](images/lstm_model_architecture.png)

### Training Performance

Training Accuracy

![LSTM Accuracy](images/lstm_training_accuracy.png)

Training Loss

![LSTM Loss](images/lstm_training_loss.png)

### Model Evaluation

Confusion Matrix

![LSTM Confusion Matrix](images/lstm_confusion_matrix.png)

---

# Model Comparison

The overall performance of both deep learning models is summarized below.

![Model Comparison](images/model_performance_comparison.png)

Both models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The Dense Neural Network provides a strong baseline classifier, while the LSTM leverages temporal relationships between consecutive weather observations, making it more suitable for sequential rainfall prediction tasks.
