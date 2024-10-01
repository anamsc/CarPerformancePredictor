# CarPerformancePredictor

## Project Overview
The objective of this project is to predict the fuel efficiency (measured in miles per gallon - mpg) of cars based on various features such as:
- Number of cylinders
- Displacement
- Horsepower
- Weight
- Acceleration
- Model year
- Origin
- Car name

We applied machine learning techniques to build predictive models using these characteristics.

## Dataset
The dataset contains information about cars and their performance characteristics. The target variable is `mpg`, which represents the car's fuel efficiency. The other variables describe features of the cars (e.g., engine specifications, weight, year, and origin).

## Data Preprocessing
- **Handling Missing Values**: Missing data were identified and handled.
- **Normalization**: Certain numerical features were normalized to improve model performance.
- **Duplicate Removal**: Duplicate records were identified and removed to avoid bias in model training.
- **Exploratory Data Analysis (EDA)**: A correlation matrix was used to understand relationships between variables. Strong negative correlations with `mpg` were found for variables like `cylinders`, `displacement`, and `weight`.

## Models Implemented
Two types of models were implemented:
1. **Linear Regression**: Simple and interpretable, it attempts to model the relationship between `mpg` and the features using a linear function.
2. **Random Forest**: A robust ensemble learning method that uses multiple decision trees to improve prediction accuracy.

### Model Evaluation
The models were evaluated using:
- **Mean Squared Error (MSE)**: Measures the average squared difference between actual and predicted values.
- **R² Score**: Represents the proportion of the variance in the dependent variable explained by the model.

## Key Results
- **Best Performing Model**: Linear Regression Model 2 provided the best results with the lowest MSE and highest R² score.
- **Comparison**: While the Random Forest models also performed well, they were slightly outperformed by Linear Regression in this specific dataset.

## Conclusions
- The analysis revealed strong negative correlations between `mpg` and features such as `cylinders`, `displacement`, and `weight`.
- Linear Regression performed better than Random Forest for this dataset, making it the preferred choice based on the evaluation metrics.

## Future Work
- Explore additional machine learning models for comparison.
- Tune hyperparameters for Random Forest to further improve performance.

