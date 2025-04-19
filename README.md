# Gemstone Price Prediction

GemPricer is an end-to-end ML Pipeline that predicts gemstone prices. It incorporates data preprocessing, model training, evaluation, and experiment tracking using MLflow, with data fetched from MongoDB and integrated with tools like Comet, DVC, and Prefect.

## Features

- Data preprocessing and feature extraction
- Model training using **Linear Regression**, **Lasso**, **Ridge**, and **ElasticNet**
- Model evaluation using metrics like **RMSE**, **MAE**, and **R²**
- **MLflow** integration for experiment tracking
- **MongoDB** integration for fetching data
- **DVC** for data version control
- **Comet** for experiment tracking and visualization
- **Prefect** for workflow management


## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/om2007464/End-to-End-MLOPs-project.git
   cd End-to-End-MLOPs-project

   python -m venv venv
   source venv/bin/activate

   pip install -r requirements.txt
   ```

2. **Running the Application**:

   Web UI: To start the Flask web application, run
   ```
   python gempricer.py
   ```

3. **Model Training Pipeline**: 
   ```
   python gemstone_training_pipeline.py
   ```
## MongoDB Configuration

Ensure MongoDB is installed and running. Use the MongoDB URI to connect and fetch data into the project. Update your ```data_ingestion.py``` or any relevant configuration with your MongoDB URI.

## MLflow Configuration

MLflow is integrated for tracking experiments, logging model parameters, metrics, and saving the best models. To start using MLflow:

Make sure to configure the ```MLFLOW_TRACKING_URL``` properly.
The default is usually local, but it can be changed to a remote server if needed.



## Prefect Dashboard :
![image](https://github.com/user-attachments/assets/da02e7e6-7614-4b4e-8780-d4619eff9b82)


Flow run in prefect :
![image](https://github.com/user-attachments/assets/9acef5a5-e51a-439c-a572-d0e5e00bbec8)


Monitor experiment in CometML dashboard :
![image](https://github.com/user-attachments/assets/75648d6b-6ccf-4a84-8e09-6bb1a3b02586)

---
This project is based on [Om](https://github.com/om2007464/End-to-End-MLOPs-project)'s end-to-end ML repository



