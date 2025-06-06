# Customer Churn Prediction using Artificial Neural Network (ANN)

This project is a web application built with Streamlit that predicts customer churn using an Artificial Neural Network (ANN). The model is trained on customer data and can help businesses identify customers who are likely to leave.

## Features
- Predicts the probability of customer churn based on user input.
- Uses a trained ANN model (`model.h5`).
- Handles categorical variables with pre-trained encoders.
- Scales input features for accurate predictions.
- User-friendly web interface built with Streamlit.

## Requirements
- Python 3.7+
- Streamlit
- TensorFlow
- scikit-learn
- pandas
- numpy

## Setup
1. **Clone the repository** (or download the project files):
   ```bash
   git clone <repository-url>
   cd annclassification
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   If `requirements.txt` is not available, install manually:
   ```bash
   pip install streamlit tensorflow scikit-learn pandas numpy
   ```

3. **Ensure the following files are present in the project directory:**
   - `app.py` (the Streamlit app)
   - `model.h5` (the trained ANN model)
   - `label_encoder_gender.pkl` (LabelEncoder for gender)
   - `onehot_encoder_geo.pkl` (OneHotEncoder for geography)
   - `scaler.pkl` (StandardScaler for input features)

## Running the App
Start the Streamlit app with the following command:
```bash
streamlit run app.py
```
This will open the app in your default web browser.

## Usage
1. Fill in the customer details in the sidebar or main form:
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
2. Click to get the churn probability and prediction.

## How it Works
- The app encodes and scales the input data using pre-trained encoders and scaler.
- The processed data is fed into the ANN model to predict the probability of churn.
- The result is displayed as a probability and a message indicating if the customer is likely to churn.

## Notes
- Make sure all model and encoder files are present in the same directory as `app.py`.
- The model and encoders must be trained on data with the same structure as the input form.

## License
This project is for educational purposes. Please check the repository for license details. 