# Forest Fire Weather Index Prediction System

A machine learning-powered web application that predicts the **Forest Fire Weather Index (FWI)** using meteorological and environmental conditions. The project combines data preprocessing, predictive modeling, and a user-friendly Flask interface to deliver real-time fire risk assessments.

## Project Overview

This application uses a trained **Ridge Regression** model to estimate the Forest Fire Weather Index based on weather and vegetation-related parameters. Users can enter environmental measurements through a web interface and instantly receive a predicted FWI value.

The project demonstrates the complete machine learning workflow, including data preprocessing, model training, serialization, deployment, and web application development.

## Features

* Real-time Forest Fire Weather Index prediction
* Interactive web interface built with Flask
* Input validation through HTML forms
* Standardized feature preprocessing using Scikit-learn
* Trained Ridge Regression model for prediction
* Fast and lightweight deployment
* User-friendly prediction dashboard

## Input Parameters

The model predicts FWI using the following environmental factors:

* Temperature (°C)
* Relative Humidity (RH)
* Wind Speed (Ws)
* Rainfall (Rain)
* Fine Fuel Moisture Code (FFMC)
* Duff Moisture Code (DMC)
* Initial Spread Index (ISI)
* Fire Class Indicator
* Region

These variables are standardized using a pre-trained StandardScaler before being passed to the machine learning model.

## Machine Learning Pipeline

### Data Preprocessing

* Data cleaning and preparation
* Feature scaling using StandardScaler
* Training and testing dataset split

### Model Development

* Ridge Regression implemented using Scikit-learn
* Hyperparameter tuning for improved generalization
* Model serialization using Pickle

### Deployment

* Flask backend for handling requests
* HTML templates for user interaction
* Pickled model and scaler loaded during application startup
* Real-time prediction generation

## Technologies Used

* Python
* Flask
* Scikit-learn
* NumPy
* Pandas
* HTML/CSS
* Pickle

## Skills Demonstrated

* Machine Learning Model Development
* Regression Analysis
* Feature Scaling and Data Preprocessing
* Model Serialization and Deployment
* Flask Web Development
* End-to-End ML Application Development
* RESTful Request Handling
* Productionizing Machine Learning Models

## Project Structure

```text
forest-fire-prediction/
│
├── application.py          # Flask application
├── models/
│   ├── ridge.pkl           # Trained Ridge Regression model
│   └── scaler.pkl          # StandardScaler object
│
├── templates/
│   ├── index.html          # Landing page
│   └── home.html           # Prediction page
│
├── requirements.txt
└── README.md
```

## Run Locally

### Clone the Repository

```bash
git clone <repository-url>
cd forest-fire-prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Start the Application

```bash
python application.py
```

Open your browser and visit:

```text
http://localhost:5000
```

## Applications

* Forest fire risk assessment
* Environmental monitoring systems
* Climate and weather analytics
* Disaster management support tools
* Educational demonstrations of machine learning deployment

## Future Improvements

* Deploy on Render, Railway, or AWS
* Add interactive visualizations and dashboards
* Implement multiple regression models for comparison
* Integrate real-time weather APIs
* Add model monitoring and performance tracking

## Author

**Muhammad Suleman**

GitHub: https://github.com/MUHAMMAD-SULEMAN-10

## License

This project is open-source and available for educational and research purposes.
