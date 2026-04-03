# Student Math Score Prediction - End-to-End ML Project

## Overview

This project is an end-to-end Machine Learning pipeline that predicts a student’s Math Score based on various academic and demographic factors.

It demonstrates how to move from data preprocessing → model training → deployment using a web application, making it a complete production-style ML project.

⸻

## Problem Statement

The objective is to predict a student’s math performance based on features such as:
	•	Gender
	•	Race/Ethnicity
	•	Parental level of education
	•	Lunch type
	•	Test preparation course
	•	Reading & Writing scores

This helps in:
	•	Identifying students needing academic support
	•	Improving performance strategies
	•	Enabling data-driven education insights

⸻

## Solution Approach

1. Data Ingestion
	•	Load dataset from source
	•	Split into train/test datasets

2. Data Transformation
	•	Handle missing values
	•	Encode categorical features
	•	Feature scaling
	•	Pipeline creation

3. Model Training
	•	Linear Regression
	•	Decision Tree
	•	Random Forest
	•	Gradient Boosting

4. Model Evaluation
	•	R² Score
	•	Mean Absolute Error (MAE)
	•	Mean Squared Error (MSE)

Best model selected based on performance metrics.

## Web Application
The project includes a Flask-based web interface where users can:
	•	Input student details
	•	Predict math score instantly

## Project Architecture
Data → Preprocessing → Model Training → Model Saving → Web App → Prediction

### Project Structure

```text
mlproject/
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   ├── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   ├── train_pipeline.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── notebooks/
│   └── EDA.ipynb
│
├── templates/
│   └── index.html
│
├── application.py
├── requirements.txt
├── setup.py
└── README.md
