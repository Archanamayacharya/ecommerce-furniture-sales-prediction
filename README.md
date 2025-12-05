# ecommerce-furniture-sales-prediction
EDA, feature engineering, and machine learning to predict furniture sales in e-commerce

# E-commerce Furniture Sales Prediction

## 📌 Overview
This project analyzes an e-commerce furniture dataset to understand sales patterns, pricing impact, discount effects, and product attributes. Feature engineering—including TF-IDF text features—was applied, and a Random Forest regression model was built to predict the number of items sold.

📊 Dataset Size: 2,000 rows (1,549 after cleaning)  
👩‍💻 Author: Archana Anil Mayacharya

---

## ✅ Problem Statement
Predict the number of furniture items sold based on product attributes such as:
- Price & original price
- Discount percentage
- Product tags
- Product title text features

---

## 🛠 Tools & Technologies
- Python  
- Google Colab  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Power BI (Dashboard)

---

## 🔄 Project Workflow
### 1. Data Cleaning
- Removed special characters from price fields
- Converted prices to numeric values
- Handled missing values and duplicates
- Filtered invalid sales records (sold > 0)

### 2. Feature Engineering
- Created discount percentage feature
- Encoded tag text using LabelEncoder
- Extracted TF-IDF features (top 50 keywords) from product titles
- Combined numeric, categorical, and text-based features

### 3. Exploratory Data Analysis
- Distribution of items sold
- Price vs sales relationship
- Original price vs sales
- Correlation heatmap

### 4. Machine Learning
- Model: Random Forest Regressor
- Target: number of items sold
- Train-test split: 80/20
- Feature scaling using StandardScaler

---

## 📈 Model Performance
| Metric | Value |
|------|------|
| MAE | 55.21 |
| RMSE | 573.69 |
| R² Score | 0.03 |

**Note:** Low R² indicates sales are influenced by additional external factors not present in the dataset.

---

## 🔍 Feature Importance Insights
Top influential features:
- Keywords in product titles (e.g., *stand*, *adjustable*, *desk*)
- Discount percentage
- Price & original price

Text-based features had a stronger influence than price alone.

---

## 💡 Key Insights
- Most furniture products have low sales; few high-demand items dominate
- Discounts significantly influence purchase behavior
- Product descriptions and keywords matter more than price alone

---

## 🚀 Future Improvements
- Include ratings, reviews, and shipping details
- Experiment with Gradient Boosting / XGBoost
- Hyperparameter tuning with GridSearchCV
- Deploy insights via interactive dashboard
