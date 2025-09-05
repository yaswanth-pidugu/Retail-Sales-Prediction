# 🛒 Retail Sales Prediction

## 📌 Overview
This project focuses on forecasting **daily sales for Rossmann stores in Germany** for up to six weeks in advance.  
By leveraging machine learning, we aim to support store managers with **data-driven decision making** instead of relying on manual predictions.

---

## 🎯 Business Problem
Rossmann managers currently predict sales manually.  
Accurate sales forecasting enables:
- 📦 Better **inventory management**
- 💰 Smarter **promotion planning**
- 🏪 Optimized **store operations**
- 📊 Improved **budget allocation**

---

## 📂 Project Structure

- **notebooks/** – contains Jupyter notebooks with full workflow  
  - `Retail_Sales_Prediction.ipynb` – main notebook for the project  

- `requirements.txt` – Python dependencies  
- `README.md` – project documentation  
- `.gitignore` – files/folders to ignore in Git


---

## 🔑 Approach
1. **Data Cleaning**  
   - Handled missing values  
   - Removed closed-store records  

2. **Feature Engineering**  
   - Extracted date parts (year, month, week, weekday)  
   - Encoded promotions, holidays, competition distance  
   - Created lag features to capture seasonality  

3. **Exploratory Data Analysis (EDA)**  
   - Sales trends across time, stores, and promotions  
   - Seasonality patterns and competition impact  

4. **Modeling**  
   - Linear Regression, Lasso Regression  
   - Decision Tree Regressor, Random Forest Regressor  
   - Hyperparameter tuning using RandomizedSearchCV  

5. **Evaluation Metrics**  
   - MAE (Mean Absolute Error)  
   - RMSE (Root Mean Squared Error)  
   - MAPE (Mean Absolute Percentage Error)  
   - R² Score  

---

## 🚀 Results
- **Random Forest** achieved the best performance  
- **MAPE = 5.65%**, **MAE ≈ $376**, **R² = 0.95**  
- Sales were strongly influenced by:
  - **Promotions** (up to +100% boost)  
  - **Seasonality** (Christmas peak in Nov–Dec)  
  - **Competition distance**  
  - **Store type**  

---

## 📈 Key Insights
- Stores running promotions saw **significant sales growth**  
- Seasonal peaks align with holidays and weekends  
- Stores farther from competitors generally had higher sales  
- Store Type A = highest sales volume, Type D = highest spend per customer  

---

## ⚙️ How to Run
Clone the repo and install dependencies:
```bash
git clone https://github.com/your-username/Retail-Sales-Prediction.git
cd Retail-Sales-Prediction
pip install -r requirements.txt
