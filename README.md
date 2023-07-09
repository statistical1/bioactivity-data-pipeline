# Bioactivity Data Pipeline

This repository contains the code and configuration for a bioactivity data pipeline, which collects data from EEG and EMG hardware, processes and stores this data both locally and in the AWS cloud, and provides access to the processed data via a secure web-based dashboard.

## Directory Structure

- `hardware-interface/`: Contains the drivers and configurations for the EEG and EMG hardware.
- `local-server/`: Contains scripts for local data processing, interfacing with the local database, and syncing data to AWS.
- `aws-cloud/`: Contains scripts and configuration files for data storage (S3), data processing (EMR, Lambda), and machine learning (SageMaker).
- `web-dashboard/`: Contains scripts for managing the API Gateway, lambda functions for API requests, and the static files for the web dashboard.


bioactivity-data-pipeline/  
|  
|-- hardware-interface/  
|   |-- EEG-interface/  
|   |   |-- README.md  
|   |   |-- eeg_driver.py  
|   |   |-- eeg_config.json  
|   |  
|   |-- EMG-interface/  
|   |   |-- README.md  
|   |   |-- emg_driver.py  
|   |   |-- emg_config.json  
|  
|-- local-server/  
|   |-- README.md  
|   |-- local_database.py  
|   |-- local_processing.py  
|   |-- data_sync_aws.py  
|  
|-- aws-cloud/  
|   |-- data-storage/  
|   |   |-- README.md  
|   |   |-- s3_config.json  
|   |   |-- s3_data_upload.py  
|   |  
|   |-- data-processing/  
|   |   |-- README.md  
|   |   |-- emr_config.json  
|   |   |-- emr_processing.py  
|   |   |-- lambda_functions/  
|   |   |   |-- README.md  
|   |   |   |-- data_cleaning_lambda.py  
|   |   |   |-- analytics_lambda.py  
|   |  
|   |-- machine-learning/  
|   |   |-- README.md  
|   |   |-- sagemaker_config.json  
|   |   |-- sagemaker_training.py  
|   |   |-- sagemaker_prediction.py  
|  
|-- web-dashboard/  
|   |-- README.md  
|   |-- api_gateway_config.json  
|   |-- api_functions/  
|   |   |-- get_data.py  
|   |   |-- post_data.py  
|   |-- static/  
|   |   |-- index.html  
|   |   |-- js/  
|   |   |-- css/  
|  
|-- README.md  
|-- .gitignore  
