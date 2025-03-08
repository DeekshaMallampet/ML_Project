# 🚗 Car Price Prediction using Machine Learning

## 🌟 Overview
Predicting car prices accurately is crucial for both buyers and sellers. This **Car Price Prediction** project leverages machine learning models to estimate car prices based on a variety of attributes. By analyzing key vehicle features such as engine specifications, fuel type, and body style, this project aims to provide an accurate pricing model that can be used in the automotive industry.

## 📊 Dataset
- **Source**: `CarPrice_Assignment.csv`
- **Number of Features**: The dataset contains multiple attributes that describe a car, such as:
  - Engine size, horsepower, fuel type, car body style, number of doors, drive wheel type, and more.
- **Target Variable**: `price` (car price in USD)
- **Objective**: To build a model that predicts a car's price based on its attributes.

## 🛠️ Tech Stack
This project utilizes a variety of data science tools:
- **Programming Language**: Python 🐍
- **Libraries**:
  - **Data Processing**: Pandas, NumPy
  - **Data Visualization**: Matplotlib, Seaborn
  - **Machine Learning**: Scikit-Learn

## 🔍 Workflow
### 📌 Step 1: Data Preprocessing
- **Handling Missing Data**: Checked for missing values and handled them appropriately.
- **Feature Extraction**: Extracted **brand name** and **model** from the `CarName` column to provide more relevant features.
- **Encoding Categorical Features**: Used **Label Encoding** to convert categorical data into numerical values for model compatibility.
- **Feature Selection**: Removed redundant or non-informative columns like `CarName` to improve model efficiency.

### 🏗️ Step 2: Feature Engineering
- **Derived New Features**: Created **brand-based features** to enhance prediction accuracy.
- **Categorical Encoding**: Transformed non-numeric features into meaningful numerical representations.
- **Outlier Detection & Treatment**: Identified and addressed extreme values that could impact model performance.

### 📉 Step 3: Feature Scaling
- **Standardization**: Used **StandardScaler** to normalize numerical variables, ensuring uniform scale across different attributes.

### 📊 Step 4: Exploratory Data Analysis (EDA)
EDA helps in understanding the dataset before applying ML models:
- **Distribution Analysis**:
  - Plotted histograms and KDE plots to visualize the distribution of numerical features.
  - Analyzed the **price distribution** to check for skewness.
- **Correlation Analysis**:
  - Generated a **heatmap** to identify relationships between features.
  - Found that **engine size, horsepower, and curb weight** have a strong positive correlation with car price.
- **Categorical Feature Analysis**:
  - Used count plots to visualize the distribution of categorical features like **fuel type, engine type, and drive wheels**.

### 🚀 Step 5: Model Training & Evaluation
To identify the best regression model for price prediction, we implemented and compared five machine learning algorithms:

1️⃣ **Linear Regression** 🤖 - A simple yet effective baseline model.
2️⃣ **Lasso Regression** 🔗 - Helps in feature selection by penalizing less important features.
3️⃣ **Ridge Regression** 📏 - Regularized regression to reduce overfitting.
4️⃣ **Decision Tree Regression** 🌳 - A tree-based model that captures non-linear relationships.
5️⃣ **Random Forest Regression** 🌲 - An ensemble method that improves accuracy and reduces variance.

#### 📊 Model Evaluation Metrics:
To compare model performance, we used:
- **R-squared (R²) Score**: Measures how well the model explains variance in car prices.
- **Mean Squared Error (MSE)**: Evaluates how close predictions are to actual prices.
- **Performance Summary**: Created a comparison table to analyze each model’s strengths and weaknesses.

## 🔥 Results & Insights
- **Training & Testing Split**: The dataset was split into **80% training and 20% testing**.
- **Best Performing Model**: **Random Forest Regression** achieved the highest R² score, making it the most accurate model for price prediction.
- **Key Insights**:
  - **Engine size, horsepower, and curb weight** had the strongest influence on car price.
  - **Fuel type and body style** played a minor but noticeable role in pricing.
  - **Regularized models (Lasso & Ridge)** helped in reducing overfitting but had slightly lower accuracy than ensemble models.

## 💻 How to Run the Project
Want to try it yourself? Follow these steps:
1. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
2. **Run the Jupyter Notebook or Python script.**
3. **Analyze predictions and model performance!**

## 🚀 Future Enhancements
- 🎯 **Optimize models using Hyperparameter Tuning** to improve accuracy.
- 🌐 **Deploy the model as a web-based application** for real-time car price estimation.
- 🤖 **Experiment with Deep Learning approaches** to capture complex relationships in the data.
- 📈 **Feature Selection Techniques** such as **PCA (Principal Component Analysis)** to improve efficiency and reduce dimensionality.

## 📬 Get in Touch
Have questions, feedback, or ideas for improvement? Feel free to reach out! 🚀🚗

