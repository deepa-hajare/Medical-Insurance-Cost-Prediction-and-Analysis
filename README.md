# Medical-Insurance-Cost-Prediction-and-Analysis

## Project Overview

The Medical Insurance Cost Prediction and Customer Data Analytics project is a Machine Learning project that analyzes medical insurance data and predicts insurance charges based on customer-related features.

The project explores relationships between age, BMI, smoking status, and insurance charges. It trains and compares multiple regression and classification models and uses clustering to group customers based on their insurance-related features.

The project is implemented in a Jupyter Notebook using Python and Scikit-learn.

## Objectives

- Explore and analyze medical insurance data using Exploratory Data Analysis (EDA).
- Check missing values and duplicate records.
- Analyze the relationship between customer features and insurance charges.
- Convert categorical features into numerical representations.
- Scale numerical features before model training.
- Split the dataset into training and testing sets.
- Train and compare multiple regression algorithms.
- Classify insurance charges into high-cost and normal-cost categories.
- Group customers using clustering techniques.
- Evaluate model performance using suitable metrics and visualizations.
- Predict estimated insurance charges for a new customer.

## Algorithms Used

The project implements the following Machine Learning algorithms.

### Regression Algorithms

- **Linear Regression:** Predicts insurance charges using customer features.
- **Polynomial Regression:** Models nonlinear relationships between features and insurance charges.
- **K-Nearest Neighbors (KNN) Regression:** Predicts charges based on similar customers.
- **Support Vector Regression (SVR):** Predicts continuous insurance costs using Support Vector Machines.

### Classification Algorithms

- **Logistic Regression:** Classifies customers into high-cost and normal-cost categories.
- **K-Nearest Neighbors (KNN) Classifier:** Classifies customers based on neighboring examples.
- **Support Vector Classifier (SVC):** Performs high-cost versus normal-cost classification.

### Clustering Algorithm

- **K-Means Clustering:** Groups customers into three clusters based on their insurance-related features.

## Tools and Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset

The project uses the Medical Cost Personal Dataset available on Kaggle.

**Dataset Link:** https://www.kaggle.com/datasets/mirichoi0218/insurance

The dataset contains the following features:

| Feature | Description |
|---|---|
| `age` | Age of the insured person |
| `sex` | Sex of the insured person |
| `bmi` | Body Mass Index |
| `children` | Number of dependent children |
| `smoker` | Smoking status |
| `region` | Residential region |
| `charges` | Medical insurance charges |

The `charges` column is the target variable for regression models.

## Project Workflow

### 1. Load the Dataset

Loads `insurance.csv` using Pandas and examines the dataset's structure, columns, and sample records.

### 2. Data Cleaning

Checks for missing values and duplicate records before analysis.

### 3. Exploratory Data Analysis (EDA)

- Examines descriptive statistics.
- Visualizes the distribution of insurance charges.
- Compares insurance costs for smokers and non-smokers.
- Studies the relationship between BMI and insurance charges.
- Identifies patterns in the dataset through graphs.

### 4. Data Preprocessing

- Separates input features from the target variable.
- Standardizes numerical features such as age, BMI, and children.
- Applies One-Hot Encoding to categorical features such as sex, smoker, and region.

### 5. Train-Test Split

Splits the dataset into training and testing sets using an 80/20 ratio and `random_state=42`.

### 6. Regression Model Training

Trains Linear Regression, Polynomial Regression, KNN Regression, and Support Vector Regression to estimate medical insurance charges.

### 7. Model Evaluation and Comparison

Evaluates regression models using:

- **R² Score:** Measures how well a model explains variations in insurance charges.
- **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted charges.

Compares regression model performance using a bar chart.

### 8. Classification

Creates a high-cost and normal-cost target based on the median insurance charges in the training dataset. Logistic Regression, KNN Classifier, and SVC are trained to predict these categories.

Classification performance is evaluated using accuracy.

### 9. Customer Clustering

Applies K-Means clustering to group customers into three clusters and visualizes differences in insurance charges across these groups.

### 10. New Customer Prediction

Selects the regression model with the highest test-set R² score in the notebook and uses it to estimate insurance charges for a new customer.

## Installation

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## How to Run the Project

1. Download the dataset from Kaggle.
2. Place `insurance.csv` in the same folder as the Jupyter Notebook.
3. Install the required libraries.
4. Open a terminal in the project directory.
5. Start Jupyter Notebook:

```bash
jupyter notebook
```

6. Open `Medical_Insurance.ipynb`.
7. Run the cells sequentially from top to bottom.

## Project Structure

```text
Medical-Insurance-Project/
├── Medical_Insurance.ipynb
├── insurance.csv
└── README.md
```

If you rename the notebook, update its filename in the project structure accordingly.

## Results

The notebook prints R² scores and MAE values for the regression models and accuracy scores for the classification models. It also displays visualizations of insurance charges and customer clusters.

Actual model performance should be recorded after running the notebook. No specific accuracy or R² score is guaranteed.

## Future Improvements

- Add a correlation heatmap and detailed feature analysis.
- Improve models through hyperparameter tuning and cross-validation.
- Add actual-versus-predicted plots and residual analysis.
- Evaluate classification models using precision, recall, F1-score, and a confusion matrix.
- Add DBSCAN clustering for comparison with K-Means.
- Build an interactive Streamlit dashboard for data analysis and cost prediction.
- Deploy the trained model through a web application.

## Author

**Deepa Hajare**


