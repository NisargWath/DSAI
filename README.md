# Bank Customer Complaint Classification

This project implements a web-based application for classifying customer complaints into financial product categories using Natural Language Processing (NLP) and Logistic Regression. The app is built with Flask and uses TF-IDF for text vectorization.

## Project Overview

This project classifies customer complaints into the following categories:
- Credit Cards
- Retail Banking
- Credit Reporting
- Mortgages and Loans
- Debt Collection

The data is preprocessed by cleaning the text, tokenizing, and applying TF-IDF. Logistic Regression is then used as the classifier to predict the category based on the complaint text input.

## Table of Contents
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Features](#features)
- [Setup](#setup)
- [Usage](#usage)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)

## Technologies Used
- Python 3.x
- Flask (for web framework)
- Pandas & NumPy (for data handling)
- Scikit-learn (for ML model and text vectorization)
- NLTK (for text processing)
- HTML/CSS (for the frontend)
- Logistic Regression (for classification)

## Project Structure
```
├── app.py                # Flask web app
├── complaints.csv         # Dataset for training
├── templates/
│   └── index.html         # HTML form for user input
└── static/
    └── style.css          # Optional CSS for styling
```

## Features
- **Data Cleaning**: Removes punctuation and tokenizes complaint text.
- **TF-IDF Vectorization**: Converts text into numerical features.
- **Logistic Regression**: Classifies the complaint into one of five product categories.
- **Flask Web Interface**: Allows users to input complaints and get predictions.

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/username/complaint-classification.git
   cd complaint-classification
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Flask application:
   ```bash
   python app.py
   ```

## Usage
1. Go to `http://127.0.0.1:5000/` in your web browser.
2. Enter a customer complaint into the form.
3. Submit the form to receive a prediction for the category of the complaint.

## Results
- **Accuracy**: Logistic Regression achieved an accuracy of approximately XX% on the test data.
- **F1 Score**: The model's F1 score is approximately XX.

## Future Work
- Incorporate other models such as **Random Forest** or **BERT** to improve accuracy.
- Enhance the frontend with additional features and better styling.
- Extend the model to classify additional financial products.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

---
