# End-to-End Machine Learning Project

## Overview

This repository demonstrates a complete end-to-end machine learning workflow for a standard supervised learning task such as regression or classification. The project covers data exploration, preprocessing, model training, evaluation, and deployment as a web application.  

The pipeline is designed with modular components for scalability and maintainability, and includes CI/CD integration and cloud deployment support.

Example use cases include:
- House price prediction  
- Student performance prediction  
- Any structured tabular regression or classification problem  

If you apply this project to a specific dataset, update this section with dataset details and problem definition.

---

## Features

- Exploratory Data Analysis (EDA) using Jupyter notebooks  
- Modular data ingestion and preprocessing pipeline  
- Model training using CatBoost gradient boosting  
- Model evaluation and artifact storage  
- Web application for real-time inference  
- Logging and custom exception handling  
- CI/CD using GitHub Actions  
- Deployment-ready setup for AWS Elastic Beanstalk  

---

## Installation

### Clone the repository
```bash
git clone https://github.com/parshvak26/End-to-End-ML.git
cd End-to-End-ML
```

### Create a virtual env
```bash
python -m venv venv
```

### Activate Env
```bash
venv\Scripts\activate
```

### Install dependencies
```bash
pip install -r requirements.txt
```

### Model Training
```bash
python src/train.py
```

### This performs:
- Data ingestion
- Data transformation
- Model training with CatBoost
- Saving trained model artifacts

## Running the Web Application
### Start the Flask application:
```bash
python app.py
```

## Project Structure
```graphql
End-to-End-ML/
│
├── .ebextensions/         # AWS Elastic Beanstalk configurations
├── .github/workflows/     # CI/CD pipelines (GitHub Actions)
├── artifacts/             # Saved models and preprocessing objects
├── catboost_info/         # CatBoost training logs
├── notebook/              # Jupyter notebooks for EDA
├── src/                   # Source code
│   ├── components/        # Data ingestion, transformation, training modules
│   ├── pipeline/          # Training and prediction pipelines
│   ├── logger.py          # Logging utility
│   ├── exception.py       # Custom exception handling
│   └── utils.py           # Helper functions
│
├── templates/             # HTML templates for web app
├── app.py                 # Main web application
├── requirements.txt       # Dependencies
├── setup.py               # Package configuration
├── README.md              # Project documentation
└── .gitignore

```
