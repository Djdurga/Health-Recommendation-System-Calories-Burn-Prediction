# 🏥 Health Recommendation System & Calories Burn Prediction

This project focuses on building a **Health Recommendation System** that predicts the number of calories burned during physical activities using physiological and exercise-related parameters. The model also provides **personalized health recommendations** based on the predicted output.

---

## 🔍 Problem Statement

People often struggle to understand how their daily activities and body metrics influence calorie expenditure. This system helps users:
- Estimate calories burned
- Understand key influencing factors
- Receive customized fitness recommendations

---

## 📦 Dataset Description

The dataset contains individual biometric and exercise-related attributes.

| Feature | Description |
|--------|-------------|
| Age, Gender | Basic biological profile |
| Height, Weight, BMI | Body composition indicators |
| Duration | Time spent exercising |
| Heart Rate | Intensity of physical activity |
| Body Temperature | Physiological exertion indicator |
| **Calories (Target)** | Number of calories burned |

---

## 🛠️ Workflow & Methodology

### 1. Data Preprocessing
- Handled missing values  
- Encoded categorical variables (Gender)  
- Scaled numeric features for model stability  

### 2. Model Development
Tested multiple regression models:
- Linear Regression
- Random Forest Regressor ✅ (Best Performance)
- XGBoost Regressor

### 3. Evaluation Metrics
The best model (Random Forest) achieved:

| Metric | Score |
|-------|-------|
| **R² Score** | ~0.95 |
| MAE | Low Error |
| RMSE | Low Error |

This indicates high predictive accuracy and model reliability.

---

## 🌟 Feature Importance (Key Factors Effecting Calorie Burn)

| Rank | Feature | Impact Summary |
|------|---------|----------------|
| 1 | **Heart Rate** | Strongest indicator — higher HR leads to more calories burned |
| 2 | **Duration of Exercise** | Longer activity duration increases burn rate |
| 3 | **Body Temperature** | Indicates exertion level |
| 4 | Weight / BMI | Higher weight generally increases calorie burn |
| 5 | Age & Gender | Moderate effect |

> **Insight:** Heart Rate & Duration are the most influential contributors.

---

## 🧠 Health Recommendation System

Based on predicted calories and user metrics, the system provides:
- Suggested **workout duration and intensity**
- Personalized **diet recommendations**
- **Daily activity guidance**
- Alerts for **unsafe exertion levels**

---

## 🧱 Tech Stack

| Component | Technology Used |
|----------|----------------|
| Programming | Python |
| Data Handling | Pandas, NumPy |
| Modeling | Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Deployment (Optional) | Streamlit / Flask |

---

## 📂 Project Structure

