# Amazon_Delivery_Time_Prediction
# Amazon Delivery Time Prediction

## 📌 Project Overview
This project aims to predict delivery times for Amazon deliveries based on various factors such as:
- Store and drop-off locations
- Agent performance (age, rating)
- Environmental conditions (weather, traffic)
- Order details (time, category, vehicle used)

By leveraging **Machine Learning**, we provide an analytical approach to estimating delivery times, helping to improve **logistics efficiency**.

---

## 📂 Dataset
The dataset contains **43,648** records, each representing a delivery order with:
- **Geographical Data**: Store & drop-off latitude/longitude
- **Agent Information**: Age, rating
- **Order Details**: Date, time, pickup time, category
- **Environmental Factors**: Weather, traffic, area type
- **Target Variable**: `Delivery_Time` (minutes)

---

## 🛠️ Workflow
### 1️⃣ Data Preprocessing
- Handling missing values and outliers
- Feature engineering:
  - Encoding categorical variables (One-Hot Encoding, Label Encoding)
  - Creating new features (distance calculation, time encoding)
  - Clustering store and drop-off locations

### 2️⃣ Exploratory Data Analysis (EDA)
- Correlation analysis
- Impact of weather, traffic, vehicle type on delivery time
- Clustering analysis to identify delivery zones

### 3️⃣ Model Training & Evaluation
- **Random Forest Regressor** was chosen due to its robustness in handling categorical data and feature importance interpretation.
- Hyperparameter tuning using **GridSearchCV**.
- **Final Model Performance**:
  - **Mean Absolute Error (MAE)**: 17.99 minutes
  - **Root Mean Squared Error (RMSE)**: 23.03 minutes
  - **R² Score**: 0.8046

---

## 📊 Key Findings
- **Traffic** conditions significantly impact delivery time.
- **Store-Drop Pairs** show location-based patterns affecting efficiency.
- **Weather conditions** have a noticeable but smaller effect.
- **Vehicle Type** influences delivery times (motorcycles being the fastest).


