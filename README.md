# Bank Notes Fake/Real Classification Using Deep Learning

This project aims to classify banknotes as either *Real* or *Fake* using a Deep Learning Artificial Neural Network (ANN).

## 📄 About the Data
The dataset includes features derived from images of real and forged banknotes using Wavelet Transform. The features are:
- **VWTI**: Variance of Wavelet Transformed Image
- **SWTI**: Skewness of Wavelet Transformed Image
- **CWTI**: Curtosis of Wavelet Transformed Image
- **EI**: Entropy of Image

## 🛠️ Workflow
1. **Data Preprocessing**:
   - Splitting into training, validation, and test sets.
   - Feature scaling using `StandardScaler`.
2. **Model Design**:
   - ANN with:
     - Input layer (64 neurons, ReLU activation).
     - Hidden layers with Dropout for regularization.
     - Output layer (Sigmoid activation for binary classification).
3. **Training**:
   - Early stopping applied to avoid overfitting.
4. **Evaluation**:
   - Metrics: Accuracy, Loss.
   - Visualization: Confusion Matrix.
5. **Prediction System**:
   - Predicts if a banknote is *Real* or *Fake* based on input features.

