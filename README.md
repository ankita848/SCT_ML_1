# House Price Prediction Using Linear Regression

## 📌 Project Overview
This repository implements a simple **Linear Regression** model to predict house sale prices based on a subset of features from the **Kaggle House Prices dataset**.  
The project covers:
- Data loading & preprocessing
- Exploratory data analysis (EDA)
- Model training
- Model evaluation
- Visualization of results

---

## 📊 Dataset
- **Source:** `train.csv` from Kaggle’s *House Prices: Advanced Regression Techniques* competition  
- **Sample Size:** 1,460 observations in `train.csv`

---


## 🧮 Features Selected

## ⚙️ Requirements

Make sure you have **Python 3.x** installed along with the following libraries:


| Feature Column   | Description                                         
|------------------|-------------------------------------------
| GrLivArea        | Above grade (ground) living area (sq ft)              
| BedroomAbvGr     | Number of bedrooms above ground                       
| FullBath         | Number of full bathrooms                              
| SalePrice        | Sale price of the house *(Target)*                    



## 🛠 Methodology

### 1️⃣ Data Loading
- Imported `train.csv` using **pandas**.

### 2️⃣ Preprocessing
- Selected only the columns of interest (`GrLivArea`, `BedroomAbvGr`, `FullBath`, `SalePrice`).
- Renamed columns for readability.
- Checked for missing values and calculated basic statistics.

### 3️⃣ Data Splitting & Scaling
- Split dataset into training (90%) and testing (10%) sets using **`train_test_split`**.
- Applied **StandardScaler** to standardize feature means and variances.

### 4️⃣ Model Training
- Trained a **LinearRegression** model on the standardized training data.

### 5️⃣  Model Evaluation
- Predicted sale prices on the test set.
- Calculated:
  - **R² Score**
  - **Mean Absolute Error (MAE)**
- Plotted predicted vs. actual values with:
  - Perfect prediction reference line
  - Error bars


## 📥 Installation & Usage

### 1. Clone this repository


git clone https://github.com/ankita848/SCT_ML_1.git
cd SCT_ML_1

2. Place dataset
Make sure train.csv is in the project root directory.


Clone this repository:

git clone https://github.com/ankita848/SCT_ML_1.git
cd SCT_ML_1

Open the notebook:

jupyter notebook project.ipynb


3. Run the notebook

jupyter notebook "House Price Linear Regression.ipynb"
Execute cells sequentially to reproduce:

Data analysis

Model training

Result visualizations

📈 Results
R² Score: ~0.63 on the test set

📊 Features

Data preprocessing (handling missing values, encoding, scaling, etc.)


Visualization: The scatter plot of predicted vs. actual sale prices shows a decent fit.
A perfect prediction line (dashed red) helps visualize prediction accuracy.

🔮 Future Improvements
Feature Engineering: Add more relevant features.

Model Selection: Compare with advanced models like Ridge, Lasso, or Random Forest.



👤 Author

Ankita Das

Machine Learning Intern @ Skillcraft Technology



