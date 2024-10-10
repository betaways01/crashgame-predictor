# Crash Game Predictor

A web application for predicting crash game outcomes based on past results.

This Flask web application predicts potential outcomes in a crash game based on recent game results. It uses a pre-trained machine learning model to estimate whether the next game multiplier will exceed 2x and provides actionable advice based on the prediction.

## Features

Real-Time Prediction: Input previous game results to predict whether the next multiplier will exceed 2x.
User-Friendly Interface: Simple web form for input and clear display of predictions and advice.
Performance Metrics: Displays key model performance statistics, such as accuracy, precision, recall, and F1-score.
Historical Data: View previous predictions along with timestamps for better tracking.

## Installation

Follow these steps to get the application up and running on your local machine.

1. Clone the Repository

git clone <your-repo-link>
cd flaskapp

2. Create and Activate a Virtual Environment

python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. Install Dependencies

pip install -r requirements.txt

4. Place the Model Files

Place your pre-trained model.pkl and scaler.pkl files in the model/ directory.

flaskapp/
│
├── model/
│   ├── model.pkl
│   ├── scaler.pkl

## Usage

To run the application locally, follow these steps:

1. Run the Application

python app.py

2. Access the Web Interface

Open your browser and go to:

http://127.0.0.1:5000/

3. Input Game Results

Enter your last game results (e.g., the multipliers) into the provided text area and submit the form to receive a prediction on whether to BET NOW (multiplier likely ≥ 2x) or WAIT (multiplier likely < 2x).

## Requirements

Make sure to install the following dependencies:

	•	Flask: For the web framework.
	•	Pandas: For data handling.
	•	Pickle: To load the machine learning model.
	•	Scikit-learn: For scaling the input data.

### Model Information

The prediction model estimates whether the next game will exceed a 2x multiplier. Key performance metrics, including accuracy, precision, recall, and F1-score, are displayed within the interface:

Accuracy: 87%
Precision: 88%
Recall: 86%
F1-score: 87%

### Example confusion matrix:

[[33474, 42568],
 [33216, 42257]]


License
This project is licensed under the MIT License. See the LICENSE file for more details.
