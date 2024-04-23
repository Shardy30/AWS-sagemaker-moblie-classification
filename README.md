# Mobile Price Classification using SKLearn Custom Script in Sagemaker

This project leverages SKLearn and Sagemaker to classify mobile prices accurately. It encompasses data preprocessing, model training, evaluation, and deployment as an endpoint for real-time predictions.

## Project Overview:

- **Data Preprocessing:** The project begins by loading the dataset (`mob_price_classification_train.csv`), splitting it into training and testing sets, and uploading them to an S3 bucket for easy access during model training.

- **Model Training:** The Random Forest Classifier from SKLearn is utilized to train the model. The number of estimators and random state are adjustable hyperparameters.

- **Model Evaluation:** After training, the model's performance is evaluated on the test dataset. Metrics such as accuracy, precision, recall, and F1-score are computed to gauge the model's effectiveness.

- **Model Deployment:** Once the model proves satisfactory, it is deployed as an endpoint in Sagemaker, allowing seamless integration for real-time predictions.

## Usage Instructions:

1. **Prepare Data:** Ensure that the mobile price dataset (`mob_price_classification_train.csv`) is available.
2. **Run Script:** Execute `script.py` to initiate the model training and deployment process.
3. **Access Predictions:** Utilize the deployed endpoint (`endpoint_name`) to make predictions on new data.

Refer to the code and inline comments for detailed instructions and customization options.

## Requirements:

- Python 3.x
- SKLearn
- Sagemaker
- Pandas
- Boto3

---