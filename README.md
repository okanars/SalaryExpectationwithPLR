## Position Salaries Prediction

### Overview

This project is an investigation into predicting salaries based on job position levels. The dataset used in this analysis is sourced from Kaggle and can be accessed [here](https://www.kaggle.com/datasets/dermisfit/position-salaries). The aim is to determine the relationship between the job position levels and corresponding salaries using Linear and Polynomial Regression.

### Dataset

The dataset contains the following columns:

- **Level:** Level of the position
- **Salary:** Corresponding salary

### Analysis

1. **Data Exploration:** The code begins with reading the dataset using Pandas and visualizing the first and last few rows. A scatter plot is used to visualize the relationship between experience levels and salaries.

2. **Linear Regression Application:** Since the data does not appear to follow a linear pattern, applying Linear Regression results in an unfit line on the scatter plot. This is demonstrated by fitting a linear model and plotting the resulting regression line.

3. **Polynomial Regression Application:** To better model the non-linear relationship, Polynomial Regression is applied. A polynomial feature transformer is used to create polynomial features of degree 3, and a linear model is then fit to these transformed features. The result is a polynomial regression line that fits the data more accurately than the linear model.

4. **Prediction:** The model is used to predict the salaries of new employees with specific experience levels (4.5 and 6.5). The predicted salaries are printed as outputs:
   - Level 4.5: 83979.16666666721
   - Level 6.5: 133259.46969697333

### Visualizations

- A scatter plot is used to visualize the relationship between 'Level' and 'Salary'.
- The regression lines from both the Linear and Polynomial models are plotted on the scatter plot to visually compare their fit.

### Technologies Used

- Python
- Pandas for data manipulation
- Matplotlib for visualization
- Scikit-Learn for Linear and Polynomial Regression

### Conclusion

The analysis demonstrates that Polynomial Regression with a degree of 3 provides a better fit to the given dataset compared to Linear Regression. This project serves as a practical example of choosing the right regression model based on the underlying data patterns.

You can see the code and the results in the files included in this repository.
