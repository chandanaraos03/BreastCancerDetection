# Breast Cancer Prediction Using Logistic Regression

A machine learning application that classifies breast tumours as **benign or malignant** based on selected diagnostic measurements. The project uses Python, Scikit-learn, and Logistic Regression, with a Gradio interface for interactive predictions.

## Overview

This project demonstrates the application of supervised machine learning to a binary classification problem using breast cancer diagnostic data. A trained Logistic Regression model processes five numerical features to generate a predicted tumour classification.

**This project is intended for educational purposes only and is not a clinically validated diagnostic tool.**

## Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| Machine Learning Library | Scikit-learn |
| Classification Algorithm | Logistic Regression |
| Feature Preprocessing | Feature Scaling |
| Model Serialization | Joblib |
| User Interface | Gradio |
| Development Environment | Google Colab |
| Deployment Platform | Hugging Face Spaces |

## Input Features

The application accepts the following diagnostic measurements:

- Mean Radius
- Mean Texture
- Mean Perimeter
- Mean Area
- Mean Smoothness

These features are processed using the saved scaler before being passed to the trained classification model.

## Workflow

1. **Data Preparation:** Load the breast cancer dataset and select the relevant features.
2. **Preprocessing:** Scale the input features using the saved scaler.
3. **Model Inference:** Apply the trained Logistic Regression model to the processed inputs.
4. **Prediction:** Display the predicted tumour classification through the application interface.

## Repository Structure

```text
BreastCancerDetection/
├── app.py
├── requirements.txt
├── Breast_cancer_data.csv
├── simple_model.joblib
├── simple_scaler.joblib
├── easy_model.joblib
├── README.md
└── .gitattributes
```

*Note: The repository may contain additional model files. Retain only the files required by the application and document their purpose accurately.*

## Installation and Usage

### Prerequisites
- Python 3.10 or a compatible version
- pip

### Setup

Clone the repository:

```bash
git clone https://github.com/chandanaraos03/BreastCancerDetection.git
cd BreastCancerDetection
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

## Limitations

- Predictions are dependent on the training dataset and model quality.
- Performance metrics should be evaluated on unseen test data.
- The model has not been established as suitable for clinical use.

## Disclaimer

This application is an educational demonstration of machine learning for binary classification. Its predictions must not be used for medical diagnosis, treatment decisions, or clinical assessment.
