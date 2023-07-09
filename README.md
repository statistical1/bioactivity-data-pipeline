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
