# Insurance Charges Regression - Brett Vrtachnik

## Overview
This project applies regression modeling techniques to predict individual insurance charges based on features such as age, BMI, and smoking status. The dataset, sourced from Kaggle, includes both categorical and numerical data. Categorical features were encoded, and multiple regression models were trained and evaluated.

## Notebook
[Click here to open the notebook](https://github.com/bvrtachnik/ml_regression_bvrtachnik/blob/main/regression_bvrtachnik.ipynb)

## Dataset
- **Source:** [Medical Cost Personal Dataset on Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance)  
- **Target Variable:** `charges` (total medical cost billed to the individual)  
- **Selected Features:** `age`, `bmi`, `smoker_yes`

## Models Used
- **Linear Regression (Baseline)**
- **Random Forest Regressor**
- **Pipeline: Imputer → StandardScaler → Linear Regression**
- **Pipeline: Imputer → Polynomial Features (degree=3) → StandardScaler → Linear Regression**

## Findings
The Random Forest Regressor and the Polynomial Features pipeline both outperformed the baseline linear regression model. This showed that including nonlinearity and model complexity helped improve prediction accuracy on the test set.

# Project Setup

## Project Initialization

### Create a GitHub Repository
- Create a new repo on GitHub and add a default README.

### Clone the Repository
```shell
git clone [your-repo-url]
cd [cloned-repo]
```

### Add `.gitignore` and `requirements.txt` Files
- Add `.gitignore` and `requirements.txt` to the project.

### Create and Activate a Virtual Environment
```shell
python -m venv .venv
.\.venv\Scripts\Activate
```

### Upgrade Pip, Setuptools, and Wheel
```shell
py -m pip install --upgrade pip setuptools wheel
```

### Install Dependencies
```shell
pip install -r requirements.txt
```

### Track and Push Changes with Git
```shell
git add .
git commit -m "Initial commit"
git push origin main
```

### Launch the Notebook
```bash
jupyter notebook regression_bvrtachnik.ipynb
```