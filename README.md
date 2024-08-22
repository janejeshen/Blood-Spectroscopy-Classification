# Non-Invasive Blood Analysis Using Spectroscopic Data

## Introduction

In this challenge, I aim to advance non-invasive blood analysis techniques using Near Infra-Red (NIR) spectroscopic data. Traditional blood analysis involves collecting blood samples and performing various tests, but our goal is to leverage machine learning to analyze spectral data and classify levels of specific chemical compounds in blood samples without the need for invasive procedures.

The dataset consists of spectral data from the NIR wavelength range (950 nm to 1350 nm). Spectral data often has a high dimensionality compared to the number of data points, making it prone to overfitting. Our task is to build a machine learning model that generalizes well and performs robustly in predicting the levels of chemical compounds from spectral measurements.

## Dataset

- **Spectral Data**: Measurements of light absorption and reflection across various wavelengths.
- **Targets**: Levels of specific chemical compounds in the blood.

## Approach

I used a **Classifier Chain** approach with **Random Forest** as the base model to predict the levels of the following chemical compounds:

1. HDL Cholesterol (`hdl_cholesterol_human`)
2. Hemoglobin (`hemoglobin(hgb)_human`)
3. LDL Cholesterol (`cholesterol_ldl_human`)

### Model Details

- **Model**: Classifier Chain with Random Forest Classifier
- **Evaluation Metrics**: Accuracy, F1 Score, and Hamming Loss

### Results

**Training Metrics:**
- **HDL Cholesterol**
  - Accuracy: 1.0
  - F1 Score: 1.0
  - Hamming Loss: 0.0
- **Hemoglobin**
  - Accuracy: 1.0
  - F1 Score: 1.0
  - Hamming Loss: 0.0
- **LDL Cholesterol**
  - Accuracy: 1.0
  - F1 Score: 1.0
  - Hamming Loss: 0.0

**Test Metrics:**
- **HDL Cholesterol**
  - Accuracy: 0.9957
  - F1 Score: 0.9956
  - Hamming Loss: 0.0043
- **Hemoglobin**
  - Accuracy: 0.9951
  - F1 Score: 0.9850
  - Hamming Loss: 0.0049
- **LDL Cholesterol**
  - Accuracy: 0.9967
  - F1 Score: 0.9935
  - Hamming Loss: 0.0033

### Key Insights

- The model demonstrates strong performance on both training and test sets, with high accuracy, F1 scores, and low Hamming Loss across all target variables.
- The high training metrics indicate that the model has learned to classify the data well, while the test metrics show that the model generalizes effectively to new data.

### Future Improvements
Explore additional feature engineering techniques to further enhance model performance.
Investigate alternative machine learning models and ensemble methods.
Integrate the model into real-time spectroscopic devices for practical applications.
