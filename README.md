# 🏡 House Price Prediction Project

This repository contains a machine learning project designed to **predict residential house sale prices** using a comprehensive dataset. The goal is to develop an accurate and robust regression model capable of providing reliable real estate valuations based on various property features.

---

## ⚙️ Project Structure and Technologies

| File | Description |
| :--- | :--- |
| `House-Price-Predictions.ipynb` | The main Jupyter Notebook detailing the complete ML workflow: EDA, preprocessing, model training, and evaluation. |
| `[your_script.py]` | Any standalone Python scripts used for data cleaning or utility functions (adjust name as needed). |
| `LICENSE` | The MIT License file, defining usage rights and liability limitations for the code. |
| **Language** | Python 3.x |
| **Core Libraries** | Pandas, NumPy, Scikit-learn |
| **Data Analysis & Viz**| Matplotlib, Seaborn |
| **Key Models Used** | Ridge, Lasso, ElasticNet, XGBoost |

---

## 🔑 Methodology and Analysis

The project follows a standard machine learning workflow detailed step-by-step within the notebook:

1.  **Exploratory Data Analysis (EDA):** Visual and statistical analysis to understand feature distributions, check for multicollinearity, and identify outliers.
2.  **Data Preprocessing:** Handing **missing values** (using appropriate imputation strategies), scaling numerical features, and encoding categorical variables.
3.  **Feature Engineering:** Creating new, highly predictive features (e.g., total square footage, age of the house at sale) to enhance model performance.
4.  **Model Training & Comparison:** Training and evaluating several penalized linear models (Ridge, Lasso) and advanced ensemble methods (XGBoost, Gradient Boosting).
5.  **Hyperparameter Tuning:** Optimizing the final model to achieve the best possible performance metrics.

---

## 📊 Model Performance Summary

Multiple regression models were trained and evaluated on the test set. The models were primarily assessed based on **Root Mean Squared Error (RMSE)** (lower is better) and the **$R^2$ score** (closer to 1 is better).

| Model | RMSE (Lower is Better) | $R^2$ (Closer to 1 is Better) |
| :--- | :--- | :--- |
| **Ridge** | **0.112845** | **0.918251** |
| Lasso | 0.112914 | 0.918115 |
| ElasticNet | 0.112951 | 0.918067 |
| XGBoost | 0.118719 | 0.909184 |
| Linear Regression | 0.121444 | 0.905071 |
| Gradient Boosting | 0.123498 | 0.901828 |
| Random Forest | 0.135534 | 0.881721 |

### 🏆 Conclusion

The **Ridge Regressor** emerged as the optimal model for this prediction task, delivering the best balance of low error ($\text{RMSE} = 0.112845$) and high explanatory power ($R^2 = 0.918251$).

---

## 🚀 Getting Started

To run this analysis locally, follow these steps:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/veddantt/House-Price-Prediction.git](https://github.com/veddantt/House-Price-Prediction.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd House-Price-Prediction
    ```
3.  **Install Dependencies:** Ensure you have Python installed and install the required libraries:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn xgboost
    ```
4.  **Run the Notebook:** Open the `House-Price-Predictions.ipynb` file in Jupyter or Google Colab to view the full analysis and run the code.

---

## 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.
