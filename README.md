# Task 3
## Linear Regression
---

## Objectives

- Understand and implement simple linear regression with one feature.
- Extend to multiple linear regression using multiple features.
- Evaluate models using metrics like **MAE**, **MSE**, and **R² Score**.
- Visualize the regression line for simple regression.
- Interpret regression coefficients and their significance.

---

## Dataset

The dataset used in this project is a CSV file containing the following columns:

- `area` — Size of the house in square feet.
- `bedrooms` — Number of bedrooms.
- `bathrooms` — Number of bathrooms.
- `price` — House price (target variable).

---

##  Steps Performed

1. **Import the Dataset**
   - Loaded CSV file using `pandas`.
   
2. **Split Data**
   - Used `train_test_split()` to divide data into training and testing sets (67% and 33%).

3. **Fit Regression Models**
   - Trained both Simple Linear Regression (using `area`) and Multiple Linear Regression (using `Area`, `bedrooms`, `bathrooms`) with `scikit-learn`.

4. **Model Evaluation**
   - Evaluated models using:
     - **Mean Absolute Error (MAE)**
     - **Mean Squared Error (MSE)**
     - **R-squared (R²)**

5. **Visualization**
   - Plotted regression line for the simple linear regression model.
   ![image](https://github.com/user-attachments/assets/fb861283-1805-4cff-9b93-4cab0627fec9)

   - Plotted Prediction line for the multiple linear regression model
   ![image](https://github.com/user-attachments/assets/4d8fea78-6ab3-4b11-b8c4-832c06943746)

6. **Interpretation**
 -  Coefficients of the **Simple Linear Regression Model**:
    -  **Intercept (β₀)**: `2,466,429.84`
    -  **Slope (β₁)**: `446.85`
    >  Meaning: For every additional square foot, the predicted price increases by ~₹446.85.

---

 - Coefficients of the **Multiple Linear Regression Model**:

    | Feature    | Coefficient        |
    |------------|--------------------|
    | area       | 362.10              |
    | bedrooms   | 378,586.10         |
    | bathrooms  | 1,403,864.00       |

    -  **Intercept (β₀)**: `-370.64`

    > Interpretation:
    >- Each square foot adds ₹362.10 to the price.
    >- Each bedroom adds ~₹378,586.10.
    >- Each bathroom adds ~₹1,403,864.00.
    >- The model starts slightly negative due to intercept but adjusts based on input features.

