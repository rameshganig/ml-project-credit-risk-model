# Lauki Finance: Credit Risk Modeling

A machine learning-powered web application for credit risk assessment and scoring, built with Streamlit.

## 📊 Overview

This application helps financial institutions assess credit risk by analyzing various customer financial parameters and generating credit scores with risk ratings. The system uses a trained machine learning model to predict the probability of default and provides actionable credit scores ranging from 300 to 900.

## 🚀 Features

- **Interactive Web Interface**: User-friendly Streamlit dashboard for inputting customer data
- **Real-time Risk Assessment**: Instant calculation of default probability and credit scores
- **Credit Rating System**: Automatic categorization into Poor, Average, Good, or Excellent ratings
- **Comprehensive Input Analysis**: Considers multiple financial factors including:
  - Age and income details
  - Loan parameters (amount, tenure, purpose, type)
  - Credit history (delinquency ratio, DPD, utilization)
  - Residence type and account information

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **Backend**: Python
- **ML Framework**: Scikit-learn
- **Model Storage**: Joblib
- **Experiment Tracking**: MLflow
- **Data Processing**: Pandas, NumPy

## 📋 Prerequisites

- Python 3.8 or higher
- pip package manager

## 🔧 Installation

1. **Clone the repository**:
    ```bash
   git clone <repository-url>
   cd ml-project-credit-risk-model
    ```
   2. **Create a virtual environment** (recommended):
    ```bash
   python -m venv venv
   ```
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   3. **Install dependencies**:
  
   pip install -r requirements.txt
   ## 🎯 Usage

1. **Run the application**:
    ```bash
   streamlit run main.py
    ```
   2. **Access the web interface**:
   Open your browser and navigate to `http://localhost:8501`

3. **Input customer data**:
   - Enter age, income, and loan details
   - Provide credit history information
   - Select residence type, loan purpose, and loan type

4. **Generate assessment**:
   Click "Calculate Risk" to get:
   - Default probability percentage
   - Credit score (300-900 range)
   - Risk rating category

## 📁 Project Structure

bash
git clone <repository-url>
cd ml-project-credit-risk-model


2. **Create a virtual environment** (recommended):come
- Loan amount and tenure
- Average days past due (DPD)
- Delinquency ratio
- Credit utilization ratio
- Number of open accounts
- Residence type
- Loan purpose and type

### Output Metrics
- **Default Probability**: Likelihood of loan default (0-100%)
- **Credit Score**: Numerical score from 300 to 900
- **Risk Rating**:
  - Poor: 300-499
  - Average: 500-649
  - Good: 650-749
  - Excellent: 750-900

## 🤖 Machine Learning Pipeline

1. **Data Preprocessing**: Feature scaling and encoding
2. **Model Training**: Logistic regression with hyperparameter tuning
3. **Model Evaluation**: Performance metrics and validation
4. **Model Deployment**: Joblib serialization for production use

## 📊 MLflow Integration

The project uses MLflow for experiment tracking and model versioning:
- Experiment runs are stored in the `mlruns/` directory
- Model artifacts include trained models and preprocessing components
- Performance metrics and parameters are logged for reproducibility

## 🔒 Dependencies

Key libraries used:
- `streamlit`: Web application framework
- `scikit-learn`: Machine learning algorithms
- `pandas`: Data manipulation
- `numpy`: Numerical computing
- `joblib`: Model serialization
- `xgboost`: Gradient boosting (for model training)
- `optuna`: Hyperparameter optimization
- `imbalanced-learn`: Handling imbalanced datasets

## 📈 Model Performance

The credit risk model has been trained and validated on historical loan data with the following characteristics:
- Uses logistic regression for binary classification
- Features preprocessing with MinMax scaling
- Handles categorical variables through one-hot encoding

## 🚨 Important Notes

- The model uses dummy values for certain features during prediction to maintain feature consistency
- All monetary inputs should be in appropriate units (e.g., annual income)
- The application is designed for demonstration and educational purposes

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is part of a machine learning course and is intended for educational purposes.

## 🙏 Acknowledgments

- Built as part of Codebasics ML Course
- Uses industry-standard practices for credit risk modeling
- Inspired by real-world financial technology applications

---

**Lauki Finance** - Making credit risk assessment accessible and transparent.

bash
python -m venv venv
source venv/bin/activate # On Windows: venv\Scripts\activate


3. **Install dependencies**:
bash
pip install -r requirements.txt

## 🎯 Usage

1. **Run the application**:

bash
streamlit run main.py

2. **Access the web interface**:
   Open your browser and navigate to `http://localhost:8501`

3. **Input customer data**:
   - Enter age, income, and loan details
   - Provide credit history information
   - Select residence type, loan purpose, and loan type

4. **Generate assessment**:
   Click "Calculate Risk" to get:
   - Default probability percentage
   - Credit score (300-900 range)
   - Risk rating category

---
## 📁 File Structure

```
ml-project-credit-risk-model/
│
├── main.py # Streamlit web application
├── prediction_helper.py # ML prediction logic and utilities
├── requirements.txt # Python dependencies
├── README.md # Project documentation
│
├── artifacts/
│ └── model_data.joblib # Trained model and preprocessing components
│
├── mlruns/ # MLflow experiment tracking
│ ├── 0/
│ └── models/
│
└── pycache/ # Python cache files
```
---

## 🔍 Model Details

### Input Features
- Age
- Income
- Loan amount and tenure
- Average days past due (DPD)
- Delinquency ratio
- Credit utilization ratio
- Number of open accounts
- Residence type
- Loan purpose and type

### Output Metrics
- **Default Probability**: Likelihood of loan default (0-100%)
- **Credit Score**: Numerical score from 300 to 900
- **Risk Rating**:
  - Poor: 300-499
  - Average: 500-649
  - Good: 650-749
  - Excellent: 750-900

## 🤖 Machine Learning Pipeline

1. **Data Preprocessing**: Feature scaling and encoding
2. **Model Training**: Logistic regression with hyperparameter tuning
3. **Model Evaluation**: Performance metrics and validation
4. **Model Deployment**: Joblib serialization for production use

## 📊 MLflow Integration

The project uses MLflow for experiment tracking and model versioning:
- Experiment runs are stored in the `mlruns/` directory
- Model artifacts include trained models and preprocessing components
- Performance metrics and parameters are logged for reproducibility

## 🔒 Dependencies

Key libraries used:
- `streamlit`: Web application framework
- `scikit-learn`: Machine learning algorithms
- `pandas`: Data manipulation
- `numpy`: Numerical computing
- `joblib`: Model serialization
- `xgboost`: Gradient boosting (for model training)
- `optuna`: Hyperparameter optimization
- `imbalanced-learn`: Handling imbalanced datasets

## 📈 Model Performance

The credit risk model has been trained and validated on historical loan data with the following characteristics:
- Uses logistic regression for binary classification
- Features preprocessing with MinMax scaling
- Handles categorical variables through one-hot encoding

## 🚨 Important Notes

- The model uses dummy values for certain features during prediction to maintain feature consistency
- All monetary inputs should be in appropriate units (e.g., annual income)
- The application is designed for demonstration and educational purposes

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is part of a machine learning course and is intended for educational purposes.

## 🙏 Acknowledgments

- Built as part of Codebasics ML Course
- Uses industry-standard practices for credit risk modeling
- Inspired by real-world financial technology applications

---

**Lauki Finance** - Making credit risk assessment accessible and transparent.