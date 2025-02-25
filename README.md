In this project, I utilized the dataset provided in **laptop_data.csv** and performed the data processing tasks as specified in **Laptop Data Task.txt**. After completing all the preprocessing steps, I trained predictive models using **Linear Regression** and **Random Forest** algorithms and saved the final work in **Laptop Data.ipynb**.

### **Data Preprocessing and Feature Engineering**
1. **Cleaning and Formatting Data:**
   - Removed the 'GB' unit from the **Ram** column and converted it to an integer.
   - Removed the 'KG' unit from the **Weight** column and changed its data type to float.
   
2. **Feature Engineering:**
   - Added a new binary column **Touchscreen**, assigning **1** where a touchscreen is available and **0** otherwise.
   - Added a new binary column **IPS**, assigning **1** where IPS technology is available and **0** otherwise.
   - Split the **Resolution** column into two new columns: **X_Res** (horizontal resolution) and **Y_Res** (vertical resolution).
   - Calculated the **PPI (Pixels Per Inch)** using the formula:
     \[ ppi = \frac{\sqrt{(X_{Res}^2 + Y_{Res}^2)}}{Inches} \]
   - Extracted **CPU Name** from the **CPU** column to categorize processor types.

### **Model Training and Evaluation**
1. **Linear Regression Model:**
   - Trained a **Linear Regression** model to predict laptop prices based on available features.
   - Evaluated model performance using **Mean Absolute Error (MAE), Mean Squared Error (MSE),** and **R² Score**.

2. **Random Forest Model:**
   - Implemented a **Random Forest Regressor** to improve predictive accuracy.
   - Tuned hyperparameters like the number of estimators and maximum depth for better performance.
   - Compared model performance with **Linear Regression** using the same evaluation metrics.

### **Conclusion**
- The **Random Forest** model performed better than **Linear Regression** in terms of predictive accuracy due to its capability to capture complex relationships.
- Feature engineering played a crucial role in improving model performance.
- The project successfully demonstrated **data preprocessing, feature engineering, and machine learning model training** for laptop price prediction.

All the tasks were implemented in **Laptop Data.ipynb**, making the dataset ready for analysis and predictive modeling.

