## Loan Approval Prediction Using Decision Tree

This project is a Streamlit machine learning application for predicting whether a loan application is likely to be approved. The app uses a Decision Tree classifier trained on the provided loan approval dataset.

### Requirements
1. Setup Github account
2. Install Python 3.11+
3. Create virtual environment
```
python -m venv venv
```
4. Activate virtual environment
* Windows
```
venv\Scripts\activate
```
* Linux/MacOS
```
source venv/bin/activate
```
5. Install required packages:
```
pip install -r requirements.txt
```
### Prelude: Try Streamlit
1. Create toy application with Streamlit.
2. Push repository to GitHub.
3. Deploy on Streamlit community cloud.  

Sample application code: [toy-app.py](toy-app.py)
### Step 1: Train and Save Model
1. Perform EDA and model development on Jupyter notebook.
2. Train a Decision Tree model and register it for inference.
3. Run the training module:
```
python -m src.training --data_path data/loan_approval_dataset.csv
```
Model development notebook: [DSSI_LoanModel.ipynb](notebooks/DSSl_LoanModel.ipynb)  
Training script: [training.py](src/training.py)  
Model registry script: [model_registry.py](src/model_registry.py)
### Step 2: Create App and Load Model
1. Load the registered Decision Tree model for inference.
2. Run the Streamlit interface to collect user inputs and display the prediction result.  

Inference script: [inference.py](src/inference.py)  
Streamlit application: [app.py](app.py)
### Step 3: Test App Locally
Run and test the application locally:
```
streamlit run app.py
```
### Step 4: Deploy App Online
1. Commit repository to GitHub.
2. Deploy on Streamlit community cloud.
