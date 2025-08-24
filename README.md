House Prices Prediction (Kaggle)

This project is based on the Kaggle "House Prices: Advanced Regression Techniques" competition.  
The goal is to predict house sale prices using advanced regression models.

📂 Project Workflow

1. Data Import & Exploration
- Loaded `train.csv` and `test.csv`
- Checked dataset structure, datatypes, and missing values
- Visualized target variable distribution (`SalePrice`)

2. Data Cleaning & Feature Engineering
- Fixed inconsistent categorical values
- Dropped irrelevant columns (e.g., IDs)
- Created new features (`TotalSF`, `HouseAge`)
- Encoded categorical variables (OneHotEncoding)
- Applied log-transform on skewed numeric features
- Applied log1p transform on target (`SalePrice`)

3. Exploratory Data Analysis (EDA)
- Correlation heatmap
- Feature vs. SalePrice plots

4. Model Building
- Train-validation split
- Tested models:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Random Forest Regressor
  - Gradient Boosting (XGBoost / LightGBM)

5. Model Comparison
- Evaluated models using **RMSE (Root Mean Squared Error)**
- Compared accuracy across all models
- Selected the best-performing model

6. Final Submission
- Trained the best model on the full training dataset
- Converted predictions back from log-scale using `expm1`
- Generated `submission.csv` for Kaggle


🚀 Results
- Baseline models (Linear, Ridge, Lasso) achieved moderate performance  
- Tree-based models (Random Forest, XGBoost, LightGBM) performed better  
- Final model achieved a Kaggle public score of **~0.13–0.15 RMSE**


🛠️ Tech Stack
- Python (Pandas, NumPy, Scikit-learn)
- Matplotlib, Seaborn (Visualization)
- XGBoost / LightGBM
- Jupyter Notebook

📌 How to Run
1. Clone this repo  
   ```bash
   git clone https://github.com/your-username/house-prices-prediction.git
   cd house-prices-prediction
Install dependencies

bash
Copy
Edit
pip install -r requirements
(numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
lightgbm
)
Run the notebook house_prices_prediction.ipynb

📜 Acknowledgements
Kaggle Dataset: House Prices - Advanced Regression Techniques

yaml
Copy
Edit











Ask ChatGPT
