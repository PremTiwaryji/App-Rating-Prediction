# App-Rating-Prediction
A Machine Learning project to predict Google Play Store app ratings using Linear Regression. It includes data cleaning, EDA, and model building using Python.

---

# 📊 App Rating Prediction Project - Google Play Store Analysis

---

## 📌 Objective
The objective of this project is to build a machine learning model to predict the app rating based on various features like reviews, size, installs, and price provided in the Google Play Store dataset. This helps the Google Play Store team identify promising apps to boost their visibility in recommendations and search results.

---

## 📂 Dataset Overview
The dataset contains information about various apps, including:
- **App**: Name of the application
- **Category**: Category the app belongs
- **Rating**: Overall user rating (Target Variable)
- **Reviews**: Number of user reviews
- **Size**: Size of the app
- **Installs**: Number of downloads
- **Price**: Price of the app
- **Content Rating**: Target age group

---

## 🔧 Tools & Libraries Used
- **Python** (Jupyter Notebook / Anaconda)
- **Pandas** for data manipulation
- **NumPy** for numerical operations
- **Matplotlib & Seaborn** for data visualization
- **Scikit-learn** for machine learning tasks

---

## ⚙️ Project Workflow
### 1. Data Cleaning & Preprocessing
**Handling Missing Values**: Dropped records with null values to ensure data quality.
**Data Formatting**: 
    - Converted 'Size' to a numeric format by handling Mb and Kb values.
    - Converted 'Reviews', 'Installs', and 'Price' into numeric types for analysis.
* **Sanity Checks**: 
    - Ensured ratings are between 1 and 5.
    - Verified that Reviews do not exceed Installs.
    - Confirmed that free apps have a price of 0.

---

### 2. Exploratory Data Analysis (EDA)
* **Univariate Analysis**: Used Boxplots and Histograms to identify outliers in Price and Reviews.
* **Outlier Treatment**: Dropped apps with suspicious prices (>$200) and extremely high review counts (>2 Million) to avoid model skewness.
* **Bivariate Analysis**: Analyzed the relationship between Rating and other features like Size, Price, and Category using scatter plots and boxplots.

---

### 3. Model Building
* **Data Transformation**: Applied log transformation (np.log1p) to skewed features like Reviews and Installs.
* **Feature Engineering**: Used Dummy Encoding for categorical variables like Category and Content Rating.
* **Train-Test Split**: Divided the data into training (70%) and testing (30%) sets.
* **Algorithm**: Implemented **Linear Regression** to predict app ratings.

---

## 📈 Results
- Successfully built a predictive model for app ratings
- Achieved good **R2 score** on training and test data

---

## 📁 Files Included
- Jupyter Notebook (.ipynb)
- Project Report (.pdf)
- Dataset (.csv)
- Project Description (.rtf)

---

## 🚀 Future Improvements
- Use advanced ML models like Random Forest, XGBoost
- Hyperparameter tuning
- Feature selection

---

## Author 
**Name:** Prem Tiwary  
**Email:** premtiwary7050@gmail.com 
**LinkedIn:** www.linkedin.com/in/prem-tiwary

---

## License
This repository is for demonstration and learning purposes. Feel free to reuse the code with attribution.
