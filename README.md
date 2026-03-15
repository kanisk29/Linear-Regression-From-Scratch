# Linear Regression from Scratch (CGPA vs Package Prediction)

## Importing Required Libraries
The following libraries are imported to perform data analysis, visualization, and model evaluation.

- **matplotlib**: Used for plotting graphs and visualizations.
- **pandas**: Used for data handling and manipulation.
- **numpy**: Used for numerical computations.
- **random**: Used for selecting random samples for testing.
- **scipy.stats**: Used to create QQ plots for checking normal distribution.
- **sklearn.model_selection**: Used to split the data into training and testing sets.
- **seaborn**: Used for enhanced data visualization.
- **sklearn.metrics**: Used to evaluate model performance using various metrics.

---

## Train-Test Split
The dataset is divided into two parts:

- **Training Set**: Used to train the model.
- **Testing Set**: Used to evaluate the performance of the model.

This is done using the `train_test_split` function from `sklearn`.

---

## Data Visualization
Three plots are created to analyze the relationship and distribution of the variables.

### 1. Scatter Plot with Regression Line
A scatter plot is used to visualize the relationship between the independent variable and the dependent variable.  
A regression line is drawn over the scatter plot to show the predicted linear relationship.

### 2. QQ Plot of CGPA
A QQ (Quantile–Quantile) plot is used to check whether the CGPA values follow a normal distribution.

### 3. QQ Plot of Package
Another QQ plot is used to verify if the package values follow a normal distribution.

These plots help verify assumptions related to linear regression.

---

## Linear Regression Implementation from Scratch
Instead of using a pre-built library function, the regression model is implemented manually.

The steps followed are:

1. Calculate the **mean of the independent variable**.
2. Calculate the **mean of the dependent variable**.
3. Compute the **slope** using the covariance of the variables divided by the variance of the independent variable.
4. Compute the **intercept** using the formula derived from the means and slope.
5. Use the slope and intercept to compute predicted values.

The prediction is made using the linear equation of a straight line.

---

## Model Evaluation
To evaluate the performance of the model, several evaluation metrics are used.

### Mean Absolute Error (MAE)
Measures the average absolute difference between the predicted values and actual values.

### Mean Squared Error (MSE)
Measures the average of the squared differences between predicted and actual values.

### Root Mean Squared Error (RMSE)
The square root of MSE, giving the error in the same unit as the target variable.

### R² Score
Represents how well the regression model explains the variance in the dependent variable.  
A value closer to **1** indicates a better fit.

Example results obtained:

- Mean Absolute Error: **0.20**
- Mean Square Error: **0.08**
- Root Mean Square Error: **0.27**
- R² Score: **0.86**

These results indicate that the model performs reasonably well.

---

## Custom Prediction
The program also allows the user to input a value manually.

Example:
Enter your CGPA: 9.15


Predicted package:


4.22608240110711


This prediction is generated using the regression equation calculated from the dataset.

---

## Conclusion
This implementation demonstrates how **linear regression can be built from scratch without using machine learning libraries**.  
The approach manually calculates the slope and intercept and uses them to predict values.  
Model performance is then evaluated using standard regression metrics.
