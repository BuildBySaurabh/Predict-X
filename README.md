# PredicX – Smart File-Based Prediction System

PredicX is a Machine Learning-powered web application built with **Django** that allows users to upload datasets, explore their data, visualize patterns, train machine learning models, and generate predictions without writing code.

The goal of this project is to make data analysis and machine learning simple and accessible through an intuitive web interface.

---

## Features

### 📂 Upload Multiple File Types

PredicX supports a variety of dataset formats, including:

- CSV
- Excel (.xlsx)
- JSON
- DOC / DOCX
- PDF
- TXT

---

### 🧹 Automatic Data Preprocessing

The application automatically prepares the uploaded dataset before training.

Features include:

- Missing value handling
- Categorical data encoding
- Numeric feature scaling
- Data validation
- Dataset preview

---

### 🎯 Target Column Selection

Choose the column you want to predict, and PredicX automatically determines the appropriate machine learning algorithm based on the dataset.

---

### 🤖 Machine Learning Models

Depending on the dataset, the system automatically selects and trains one of the following models:

- Linear Regression
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

---

### 📊 Data Visualization

Generate interactive visualizations with a single click.

Available charts include:

- Correlation Heatmap
- Scatter Plot
- Histogram
- Pie Chart
- Step Plot
- Stack Plot
- 3D Scatter Plot
- 3D Surface Plot

These visualizations help users understand relationships, distributions, and trends within the dataset before training the model.

---

### 🌍 Public Dataset Sharing

Users can upload practice datasets that are publicly available for others to explore and experiment with.

---

# How It Works

```
Upload Dataset
      │
      ▼
Read File
      │
      ▼
Data Cleaning
      │
      ▼
Target Column Selection
      │
      ▼
Feature Engineering
      │
      ▼
Model Selection
      │
      ▼
Model Training
      │
      ▼
Prediction
      │
      ▼
Visualization Dashboard
```

---

# Workflow

### Step 1 — Upload Dataset

Upload a supported dataset in one of the following formats:

- CSV
- Excel
- JSON
- DOC / DOCX
- PDF
- TXT

---

### Step 2 — Dataset Preview

The application reads the file and displays:

- Dataset preview
- Number of rows
- Number of columns
- Data types
- Missing values

---

### Step 3 — Select Target Column

Choose the column you want to predict.

PredicX automatically identifies whether the problem is:

- Classification
- Regression

and selects the most suitable machine learning algorithm.

---

### Step 4 — Train the Model

The selected model is trained using the processed dataset.

The system performs:

- Data preprocessing
- Feature encoding
- Feature scaling
- Train/Test split
- Model training
- Prediction generation

---

### Step 5 — Visualize the Data

Generate charts instantly, including:

- Correlation Heatmap
- Scatter Plot
- Histogram
- Pie Chart
- Stack Plot
- Step Plot
- 3D Scatter Plot
- 3D Surface Plot

---

## Technologies Used

### Backend

- Python
- Django
- Pandas
- NumPy
- Scikit-Learn

### Frontend

- HTML5
- CSS3
- JavaScript
- Bootstrap

### Data Visualization

- Matplotlib
- Seaborn

---

# Project Structure

```
PredicX/
│
├── predicx/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
│
├── predictor/
│   ├── migrations/
│   ├── templates/
│   ├── static/
│   ├── uploads/
│   ├── views.py
│   ├── models.py
│   ├── urls.py
│   ├── ml_models.py
│   ├── preprocessing.py
│   └── visualizations.py
│
├── media/
├── requirements.txt
├── manage.py
└── README.md
```

---

# Installation

## Clone the Repository

```bash
git clone https://github.com/BuildBySaurabh/PredicX.git

cd PredicX
```

---

## Create Virtual Environment

### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv

source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Apply Database Migrations

```bash
python manage.py makemigrations

python manage.py migrate
```

---

## Create Admin Account (Optional)

```bash
python manage.py createsuperuser
```

---

## Run the Development Server

```bash
python manage.py runserver
```

Open your browser and visit:

```
http://127.0.0.1:8000/
```

---

# Technical Highlights

- Supports multiple dataset formats
- Automatic data preprocessing
- Intelligent model selection
- Classification & regression support
- Interactive data visualizations
- Automatic feature engineering
- Simple and responsive user interface
- Public dataset sharing
- End-to-end machine learning workflow

---

# Future Improvements

Planned enhancements include:

- XGBoost integration
- LightGBM support
- CatBoost models
- Hyperparameter tuning
- AutoML pipeline
- Feature importance visualization
- SHAP explainability
- Model comparison dashboard
- Dataset versioning
- User authentication
- Cloud deployment
- REST API support

---

## If you found this project useful, consider giving it a ⭐ on GitHub.
