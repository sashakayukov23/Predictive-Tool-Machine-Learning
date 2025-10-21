# Predictive Tool for SME-Education Matching at MKB Werkplaats

- **Project Title:** _Predictive Matching: Using Machine Learning to Optimise SME-Education Partnerships_
- **Author:** _Aleksandr Kaiukov_

## About the Project
This part of the project supports MKB Werkplaats in improving the success rate of SME-education collaborations, called definitive matches. By analysing past challenge data, a machine learning model was trained to estimate the likelihood of a successful match based on inputs (e.g., challenge type, institution, and company size). The deliverables include a working prediction tool, which can be used via a local web app or directly in a Jupyter/Colab Notebook.

## Contents
1. **Predictor.ipynb**
- A notebook version of the predictor. Users can test different inputs and receive probability scores. Designed for demos in Jupyter/Colab.
2. **app.py**
- A Streamlit app that runs the predictor locally in the browser. No need to modify any code, just run and use the interface.
3. **lr4_model.joblib**
- A trained Logistic Regression model pipeline. It includes all preprocessing steps (e.g., encoding, imputation).

## Note: 
The dataset used to train the model (_MKB_final_dataset.xlsx_) is excluded from the repository due to privacy. 

# How to Run the Web App Locally
**Requirements:** Python 3.8 or higher installed; pip (Python package installer)

**1. Download Files:** Save _app.py_ and _lr4_model.joblib_ into a folder on your computer.

**2. Open Command Prompt (CMD):** Navigate to the folder using _cd_, for example: _C:\Users\name\Downloads\mkb_app_

**3. Install dependencies (only once):** _pip install streamlit pandas joblib openpyxl_

**4. Run the app:** _streamlit run app.py_

**5. The app will open in your browser.** You can input values and instantly see the predicted match probability.


<img width="1920" height="1080" alt="MKB-Python-Predictor" src="https://github.com/user-attachments/assets/ade7bbb9-fcc4-47d0-984a-6ddd1b9ce041" />

<img width="1920" height="1080" alt="MKB-Web-Predictor" src="https://github.com/user-attachments/assets/279a27b4-de24-4901-a767-464e478fb34f" />
