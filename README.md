# Dogs vs. Cats CNN Classifier

## Overview
This project features a complete, end-to-end deep learning pipeline built in Google Colab. It seamlessly integrates the Kaggle API for automated data ingestion and preprocessing, culminating in a custom Convolutional Neural Network (CNN) built with TensorFlow and Keras. The resulting model efficiently processes raw data to classify images of dogs and cats, demonstrating practical skills in computer vision, automated workflow design, and model training.

## Prerequisites
Before running this notebook, ensure you have the following:
* A Google account to access Google Colab.
* A Kaggle account.
* A Kaggle API token (`kaggle.json` file). 
  > **Note:** You can generate this by navigating to your Kaggle Account settings and clicking **Create New API Token**.

## Usage Instructions

**Step 1: Run the Environment Setup**
Execute the first cell in the notebook. This imports the `files` module from `google.colab` and triggers a file upload widget. 

**Step 2: Authenticate with Kaggle**
When prompted by the widget, upload your `kaggle.json` file. The script will automatically:
* Create a hidden `~/.kaggle` directory.
* Move your uploaded `kaggle.json` file into this directory.
* Apply `chmod 600` permissions to the file to secure your API credentials.

**Step 3: Download and Extract the Dataset**
Run the next cell to execute shell commands that:
* Download the `salader/dogsvscats` dataset via the Kaggle CLI.
* Unzip `dogsvscats.zip` directly into your Colab workspace, populating it with the required training images (e.g., `train/dogs/` and `train/cats/`).

**Step 4: Train the Model**
Continue running the subsequent cells to initialize the Keras deep learning pipeline. The notebook will preprocess the image data, build the CNN architecture, and train the binary image classification model.

## Technical Stack
* **Environment:** Google Colab / Jupyter Notebook
* **Language:** Python 3
* **Libraries:** TensorFlow, Keras
* **Accelerator Setup:** Configured to support GPU acceleration (T4)
