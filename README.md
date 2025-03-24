# Datascience_Project


### Workflow-Ml Pipeline
# Basic Data Science Pipeline with Flask API

## Problem Statement

This project demonstrates a basic data science pipeline that:
- **Ingests data** from a source.
- **Transforms** the raw data into a suitable format.
- **Trains** a machine learning model.
- **Evaluates** the performance of the model.
- **Predicts** outcomes for new data.

The goal is to deploy these functionalities as a Flask API, allowing users to interact with the pipeline remotely.

## Repository Structure

- **app.py**: Flask application that exposes endpoints for triggering pipeline stages and making predictions.
- **pipeline/**
  - **data_ingestion.py**: Code to load raw data.
  - **data_transformation.py**: Code to preprocess and transform the data.
  - **data_validation.py**: Code to validate the input data.
  - **model_training.py**: Code to train the machine learning model.
  - **model_evaluation.py**: Code to evaluate the trained model.
  - **prediction.py**: Code to perform predictions using the trained model.
- **requirements.txt**: Contains Python dependencies.

## Setup

1. **Install Dependencies**

   Ensure you have Python installed, then run:

   ```sh
   pip install -r requirements.txt
   ```

2. **Configure the Project**

   Adjust any configurations (such as data source paths or model parameters) within the respective pipeline scripts if needed.

## Running the Application

1. **Run the Pipeline:**

   You can run individual pipeline stages by executing the scripts in the `pipeline/` directory, for example:

   ```sh
   python pipeline/ingestion.py
   python pipeline/transformation.py
   python pipeline/training.py
   python pipeline/evaluation.py
   ```

2. **Start the Flask API:**

   Launch the Flask application to handle predictions and trigger pipeline stages as needed:

   ```sh
   python app.py
   ```

3. **API Endpoints Examples:**

   - `GET /` - Home endpoint.
   - `POST /predict` - Submit data for prediction.
   - `POST /train` - Trigger training (if needed).


