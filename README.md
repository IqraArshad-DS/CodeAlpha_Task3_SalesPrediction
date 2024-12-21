# Sales Prediction using Python 

This repository contains the implementation of the **Sales Prediction** task, completed as part of Task 3 for the **CodeAlpha Internship**. The objective of this project is to predict the sales of a product based on advertising expenditure on TV, Radio, and Newspaper.

---

## **Overview**
Predicting product sales is a critical application in marketing and business strategy. Using machine learning, we trained regression models to predict sales based on advertising expenditure. The **Gradient Boosting Regressor** was chosen as the final model for its high accuracy and robust performance.

---

## **Workflow**
1. **Data Preprocessing**:
   - Cleaned the dataset by handling missing values and removing unnecessary columns (e.g., `Unnamed: 0`).
   - Engineered new interaction features (`TV_Radio`, `TV_Newspaper`, `Radio_Newspaper`) for better prediction.
   - Removed outliers using the IQR method to improve model generalization.
   - Scaled features using `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**:
   - Visualized feature correlations using heatmaps and pair plots.
   - Identified strong relationships between advertising on **TV** and **Radio** with sales.

3. **Model Training and Evaluation**:
   - Trained multiple regression models:
     - **Linear Regression**
     - **Random Forest Regressor**
     - **Gradient Boosting Regressor**
   - Evaluated models based on:
     - **R² Score**
     - **Mean Absolute Error (MAE)**
     - **Root Mean Squared Error (RMSE)**
   - The **Gradient Boosting Regressor** achieved the best performance:
     - **R² Score**: 0.99
     - **MAE**: 0.34
     - **RMSE**: 0.43

4. **Model Saving and Prediction**:
   - Saved the trained Gradient Boosting model as `final_gradient_boosting_model.pkl`.
   - Demonstrated predictions using new advertising expenditure data.

---

## **How to Use**
1. **Clone this repository**:
   ```bash
   git clone https://github.com/YourUsername/CodeAlpha_Task3_SalesPrediction.git
2. Open the Jupyter Notebook (Sales_Prediction.ipynb) and run the cells sequentially.
3. Use the saved model (final_gradient_boosting_model.pkl) to predict sales based on new advertising data.

**Technologies Used**
- Python
- Scikit-learn
- Matplotlib, Seaborn
- Gradient Boosting Regressor

**About CodeAlpha**

This project is part of Task 3 for the CodeAlpha Internship Program.
