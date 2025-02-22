SMS Spam Detection System Using Natural Language Processing

This project is developed by Tejas Jadhav and focuses on building a spam detection system for SMS messages using deep learning techniques in TensorFlow 2. Various architectures, including Dense Network, LSTM, and Bi-LSTM, have been implemented to build and evaluate the spam detection model. The model's accuracy is compared to determine the best-performing approach.

Dataset

The SMS Spam Collection dataset from the UCI Machine Learning Repository is used for this project. It contains 5,574 SMS messages, out of which 4,827 are labeled as ham (non-spam) and 747 as spam. The dataset is split into 4,000 messages for training and 1,574 messages for testing.

Steps Involved

The following steps were followed to build the spam detection model:

Load and Explore the Data: The dataset is loaded into a Pandas DataFrame and analyzed to understand the distribution of ham and spam messages.

Prepare Train-Test Data: The messages are tokenized, and their labels are one-hot encoded. The dataset is split into 80% training and 20% testing.

Train the Spam Detection Model: The three models - Dense Network, LSTM, and Bi-LSTM - are trained using the training dataset and evaluated using a validation dataset.

Compare and Select the Final Model: The accuracy of all models is compared, and the best-performing model is selected.

Classify New Messages: The final trained classifier is used to classify new SMS messages as either ham or spam.

Installation and Usage

To use the SMS spam detection model, follow these steps:

Clone the Repository

git clone https://github.com/TejasJadhav/sms-spam-detection.git

Install Dependencies

cd sms-spam-detection
pip install -r requirements.txt

Download the Dataset

mkdir data
wget https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection -O data/spam.csv

Train the Models

Run the Jupyter Notebook script (.ipynb) to train the models and select the best one.

Run the Streamlit App

streamlit run app.py

Model Performance

The accuracy of different models is as follows:

Dense Network - 98.5%

SVM - 97.6%

Bi-LSTM - 98.8% (Best Performing Model)

LSTM - 98.6%

Streamlit App

A Streamlit web application has been created to demonstrate the final model. The app allows users to input a message and predicts whether it is ham or spam. You can access the app here:

Streamlit App Link

Conclusion

In this project, a spam detection system for SMS messages was built using deep learning techniques in TensorFlow 2. Three different architectures were explored, with Bi-LSTM achieving the highest accuracy (98.8%). The final model has been deployed as a Streamlit web app to provide a user-friendly interface for spam detection.

Developed by Tejas Jadhav

