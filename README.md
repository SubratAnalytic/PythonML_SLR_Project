# Python_Project (ML_SLR)
# Salary Prediction Web App (Simple Linear Regression)

A machine learning web application that predicts salary based on input features (such as years of experience) using a **Simple Linear Regression** model trained in Python, served through a Python backend with an HTML frontend.

## Overview

This project demonstrates the end-to-end workflow of building and deploying a Simple Linear Regression model:
- **Machine Learning Model (`SLR_MODEL.pkl`):** A trained regression model saved for fast inference without retraining on every request.
- **Backend (`app.py`):** Handles incoming form/request data, loads the serialized model, generates salary predictions, and passes results back to the interface.
- **Frontend (`templates/`):** HTML templates that collect user input and display predicted salary results cleanly.
- **Deployment Ready (`Procfile`, `requirements.txt`):** Configured with dependencies and process definitions for hosting.

## Tech Stack

- **Backend & ML:** Python, scikit-learn / NumPy / pandas (see `requirements.txt`)
- **Model Serialization:** Pickle (`SLR_MODEL.pkl`)
- **Frontend:** HTML (`templates/`)
- **Deployment:** `Procfile`

## Project Structure

```text
├── app.py              # Application entry point & prediction routing
├── SLR_MODEL.pkl       # Serialized Simple Linear Regression model
├── requirements.txt    # Python package dependencies
├── Procfile            # Process configuration for cloud deployment
└── templates/          # HTML frontend templates

Getting Started
Prerequisites
Make sure you have Python installed on your system.

**Installation & Running Locally**

1.Clone the repository:

Bash
git clone [https://github.com/SubratAnalytic/PythonML_SLR_Project.git](https://github.com/SubratAnalytic/PythonML_SLR_Project.git)
cd PythonML_SLR_Project

2.Install the required dependencies:

Bash
pip install -r requirements.txt

3.Run the application:

Bash
python app.py

4.Open in your browser:

Navigate to http://127.0.0.1:5000/ to test the salary predictor.

**How It Works**

1.The user enters their Years of Experience into the HTML form.

2.The input is sent to the Python backend (app.py).

3.The backend loads SLR_MODEL.pkl and computes the predicted salary.

4.The predicted result is rendered back onto the web page.
