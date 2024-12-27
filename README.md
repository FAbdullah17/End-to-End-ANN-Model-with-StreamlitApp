# End-to-End ANN Model with Streamlit App

This repository contains an end-to-end implementation of an Artificial Neural Network (ANN) model for predicting customer churn. The project includes data preprocessing, model training, hyperparameter tuning, and deployment using a Streamlit-based web application.

## Features
- **Data Preprocessing**: Handles categorical variables and scales numerical features using encoders and scalers.
- **ANN Model**: Implements a fully connected Artificial Neural Network using TensorFlow/Keras.
- **Hyperparameter Tuning**: Optimizes model performance using techniques such as grid search.
- **Streamlit App**: Provides an interactive interface for users to predict customer churn based on input parameters.

## project Structure
```
End-to-End-ANN-Model-with-StreamlitApp/
├── .gitignore
├── app.py                     # Streamlit app for user interaction
├── Churn_Modelling.csv        # Dataset used for training the model
├── experiments.ipynb          # Jupyter notebook for initial experiments
├── hyperparametertuningann.ipynb # Hyperparameter tuning notebook
├── label_encoder_gender.pkl   # Gender label encoder
├── LICENSE                    # License file
├── model.h5                   # Trained ANN model
├── onehot_encoder_geo.pkl     # Geography one-hot encoder
├── prediction.ipynb           # Notebook for predictions and testing
├── README.md                  # Project documentation (this file)
├── requirements.txt           # Python dependencies
├── salaryregression.ipynb     # Notebook for salary regression analysis
├── scaler.pkl                 # Scaler for numerical features
└── venv/                      # Virtual environment folder
```

## Dataset
The `Churn_Modelling.csv` file contains customer information with the following attributes:
- Geography
- Gender
- Age
- Balance
- Credit Score
- Estimated Salary
- Tenure
- Number of Products
- Has Credit Card
- Is Active Member
- Churn (Target Variable)

## Getting Started
### Prerequisites
- Python 3.8 or higher
- Virtual Environment (recommended)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.comFAbdullah17/End-to-End-ANN-Model-with-StreamlitApp.git
   cd End-to-End-ANN-Model-with-StreamlitApp
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate    # For Linux/Mac
   venv\Scripts\activate      # For Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

### Usage
- Open the Streamlit app in your browser.
- Input customer details such as geography, gender, age, balance, credit score, and more.
- View the predicted churn probability and corresponding message.

## Model Overview
The ANN model is trained using TensorFlow/Keras and saves the trained model in the `model.h5` file. Preprocessing includes:
- Encoding categorical variables (`label_encoder_gender.pkl`, `onehot_encoder_geo.pkl`)
- Scaling numerical features (`scaler.pkl`)

## Hyperparameter Tuning
The `hyperparametertuningann.ipynb` notebook demonstrates hyperparameter tuning to improve the model's performance. Key parameters such as the number of neurons, activation functions, and optimizer settings are explored.

## Contributing
Feel free to contribute by submitting a pull request. Ensure your changes align with the project's goals and structure.

## License
This project is licensed under the [Apache-2.0 license](LICENSE).

## Acknowledgments
- Dataset sourced from [Kaggle](https://www.kaggle.com/)
- Inspired by ANN tutorials and best practices in machine learning.

## Contact
For any inquiries, contact [fahadai.co@gmail.com].
