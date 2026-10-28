
# 🚗 Car Price Predictor

A Machine Learning web application that estimates automobile prices based on vehicle specifications using Lasso Regression and Streamlit.

## 📌 Project Overview

The Car Price Predictor analyzes automobile features such as engine size, horsepower, vehicle body style, fuel type, and fuel efficiency to estimate a car's price.

The application provides an interactive interface where users can enter vehicle specifications and receive a predicted price.

## 🎯 Objectives

- Predict automobile prices using Machine Learning.
- Explore important vehicle specifications.
- Clean missing and invalid data.
- Handle outliers using the Interquartile Range (IQR).
- Encode categorical features.
- Scale numeric features.
- Build an interactive web application with Streamlit.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Lasso Regression
- Streamlit
- Git and GitHub

## 📂 Project Structure

```text
Automobile-Price-Predictor/
├── app.py
├── requirements.txt
├── README.md
├── best_model.pkl
└── Automobile_data - Automobile_data.csv
```

## 📊 Dataset

The application uses an automobile dataset containing vehicle specifications and prices.

Expected filename:

`Automobile_data - Automobile_data.csv`

### Features Used

**Numerical features**
- symboling
- normalized-losses
- width
- height
- engine-size
- horsepower
- city-mpg
- highway-mpg

**Categorical features**
- make
- fuel-type
- body-style
- drive-wheels
- engine-location
- engine-type

**Target variable**
- price

Make sure your CSV contains these columns. Column names are case-sensitive in the Python code.

## ⚙️ Installation and Setup

### 1. Clone the Repository

Replace `YOUR-USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR-USERNAME/Automobile-Price-Predictor.git
```

### 2. Navigate to the Project Folder

```bash
cd Automobile-Price-Predictor
```

### 3. Create a Virtual Environment (Recommended)

```bash
python -m venv .venv
```

Activate it in Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 4. Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### 5. Run the Application

```bash
python -m streamlit run app.py
```

Open the local URL shown in your terminal, usually:

`http://localhost:8501`

## 🔄 Machine Learning Workflow

1. Load the automobile dataset.
2. Replace invalid missing-value markers.
3. Convert numeric columns to numeric types.
4. Remove records without valid target prices.
5. Remove outliers using the IQR method.
6. Impute missing numeric and categorical values.
7. Scale numeric features using StandardScaler.
8. Encode categorical features using OneHotEncoder.
9. Train a Lasso Regression model.
10. Predict car prices through the Streamlit interface.

## 🤖 Model

**Algorithm:** Lasso Regression

Lasso Regression is a linear regression technique that uses L1 regularization to penalize large coefficients. It can help reduce overfitting and perform feature selection.

The model is trained automatically when the application starts.

## 📈 Future Improvements

- Evaluate performance using MAE, MSE, RMSE, and R².
- Compare Lasso Regression with Linear Regression and Random Forest.
- Add visualizations for price distributions and feature relationships.
- Improve input validation and outlier handling.
- Deploy the application online.

## 👩‍💻 Author

**Gayatri Jagnade**

Aspiring Data Analyst | Python | SQL | Excel | Power BI | Machine Learning

## 📄 Disclaimer

Predicted prices are estimates based on the available dataset. They are not guaranteed market prices.
