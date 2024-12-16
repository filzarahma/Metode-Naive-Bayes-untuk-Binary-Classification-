# Naive Bayes Classification for Binary Prediction

This project implements a **Naive Bayes Classification** system designed to predict binary class labels based on three feature inputs (`x1`, `x2`, `x3`). The system processes training and testing data, calculates feature likelihoods, applies Laplace smoothing, and generates predictions. The implementation is provided as a **Jupyter Notebook (`.ipynb`)** format with the option to run it on **Google Colab** or locally.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [How to Use](#how-to-use)
4. [Dependencies](#dependencies)
5. [Acknowledgments](#acknowledgments)

---

## Project Overview

This project applies a **Naive Bayes Classifier** to a dataset with the following attributes:

- **Input Features**:
  - `x1`, `x2`, `x3`: Numeric features used for prediction.
- **Target Output**:
  - `y`: Binary class label (`0` or `1`).

The classifier predicts the class label for a testing dataset based on probabilities calculated from the training dataset.

### **Key Processes:**

1. **Data Loading**: Reads training and testing data from an Excel file (`traintest.xlsx`).
2. **Data Preprocessing**:
   - Converts data into a dictionary format for processing.
   - Calculates feature-specific counts for both classes (`0` and `1`).
   - Applies Laplace smoothing to prevent zero probabilities.
3. **Model Training**:
   - Calculates prior probabilities for each class.
   - Computes likelihood probabilities for each feature value using training data.
4. **Prediction**:
   - Uses the Naive Bayes formula to predict the class label for each record in the test set.
5. **Evaluation**:
   - Evaluates model accuracy using the training dataset.
6. **Output**:
   - Saves predictions to a new Excel file (`predictions.xlsx`).

---

## Features

- **Comprehensive Training and Testing Pipeline**:
  - Processes both training and testing datasets.
  - Applies Laplace smoothing for robust probability estimation.

- **Model Evaluation**:
  - Calculates and displays the model's accuracy on the training dataset.

- **Excel Output**:
  - Saves test set predictions to an Excel file for easy sharing and further analysis.

---

## How to Use

### **1. Running on Google Colab**
   - Open the notebook in Google Colab.
   - Upload the `traintest.xlsx` file to the Colab environment:
     1. Click the "Files" tab on the left-hand side.
     2. Use the upload button to upload the file.
   - Execute the notebook cells step by step to generate predictions.

### **2. Running Locally Using Visual Studio Code**
   - Install **Visual Studio Code** and the **Python Extension** from the Extensions Marketplace.
   - Install **Jupyter** support for VS Code:
     1. Open VS Code.
     2. Go to the Extensions Marketplace and search for `Jupyter`.
     3. Install the extension.
   - Ensure Python and the required libraries are installed (see [Dependencies](#dependencies)).
   - Place the `traintest.xlsx` file in the same directory as the `.ipynb` notebook file.
   - Open the `.ipynb` file in VS Code.
   - Execute the cells sequentially or click "Run All" to process the data and save the predictions to `predictions.xlsx`.

---

## Dependencies

This project requires the following Python libraries:

- **pandas**: For data manipulation and handling Excel files.
- **openpyxl**: For reading and writing Excel files.
- **Jupyter**: For running `.ipynb` notebooks.

Install dependencies using pip:
```bash
pip install pandas openpyxl notebook
```

---

## Acknowledgments

This project was developed as part of the **Introduction to Artificial Intelligence** course by:

- **Filza Rahma Muflihah (1301201261)**  
- **Ummu Husnul Khatimah (1301204120)**  

We would like to thank the course instructors for their guidance and support in completing this project.  

If you find this project helpful, feel free to use it for learning or research purposes. Feedback and contributions are always welcome!