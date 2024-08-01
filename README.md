# Personalized Banking Advertisement Generator and Email Sender

This project generates a personalized banking advertisement based on customer data using a RandomForest model and sends the generated advertisement image via email.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Customization](#customization)
- [Notes](#notes)

## Introduction

This project utilizes synthetic banking data to train a RandomForest model that predicts a customer's product preference. Based on the predicted preference, a personalized banking advertisement is generated using Azure OpenAI's DALL-E model. The generated advertisement is then sent via email as an attachment.

## Requirements

- Python 3.7+
- pandas
- numpy
- scikit-learn
- joblib
- matplotlib
- Pillow (PIL)
- requests
- openai
- smtplib
- email



## Customization

- Modify the Customer Data:
  Update the `example_data` dictionary in `generate_and_send_ad.py` to include your own customer data.

  -Change the Email Content:
  Modify the `subject` and `body` variables in `generate_and_send_ad.py` to customize the email content.

- Adjust the RandomForest Model:
  Modify the parameters of the `RandomForestClassifier` in `generate_and_train_model.py` to tune the model.

## Notes

- Security: Avoid hardcoding your email password in the script. Use environment variables or a secure method to handle credentials.
- App-Specific Password: If you're using Gmail, it's recommended to use an app-specific password instead of your main account password for security reasons.
- Model Accuracy: If the model accuracy is less than 90%, consider tuning the model parameters or using a different algorithm.

## Contact

For any questions or issues, please contact [guptavansh2404@gmail.com].

