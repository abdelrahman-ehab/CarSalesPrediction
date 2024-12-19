# Car Dataset Regression Analysis

## Project Overview
This project involves analyzing a car dataset to predict a target variable (e.g., car price or fuel efficiency) using regression models. The analysis includes data preprocessing, exploratory data analysis (EDA), feature engineering, and building regression models. Two models were implemented: Elastic Net and Decision Tree Regression, with the Decision Tree model achieving better performance.

## Dataset
The dataset contains information about various car attributes. Key columns include:
- **Make**: The manufacturer of the car.
- **Model**: The car's model.
- **Year**: The manufacturing year of the car.
- **Engine Fuel Type**: The type of fuel the car uses.
- **Engine HP**: The engine's horsepower.
- **Engine Cylinders**: The number of cylinders in the engine.
- **Transmission Type**: The type of transmission (automatic/manual).
- **Driven Wheels**: The drivetrain type (e.g., FWD, RWD, AWD).
- **Number of Doors**: The number of doors in the car.
- **Highway MPG**: Fuel efficiency on highways.
- **City MPG**: Fuel efficiency in cities.
- **Price**: The car's price (target variable).

## Steps Followed

### 1. Data Preprocessing
- **Handling Missing Values**: Missing values in numerical columns were filled with the median.
- **Feature Scaling**: StandardScaler was used to standardize numerical features.
- **Categorical Encoding**: One-hot encoding was applied to categorical variables.

### 2. Exploratory Data Analysis (EDA)
- Summary statistics and visualizations were used to understand the dataset.
- Distribution of numerical features and relationships with the target variable were analyzed.

### 3. Feature Engineering
- Highly correlated features were identified and removed to avoid multicollinearity.
  

### 4. Model Building
- Two regression models were implemented:
  - **Elastic Net Regression**: A linear model combining L1 and L2 regularization to handle multicollinearity and feature selection.
  - **Decision Tree Regression**: A non-linear model that splits data based on feature values to capture complex patterns.

### 5. Model Evaluation
- Both models were evaluated using metrics such as Mean Squared Error (MSE) and R-squared.
- The Decision Tree Regression outperformed Elastic Net Regression in terms of predictive performance.

### 6. Results
- **Elastic Net Regression**:
  - Mean Absolute Error: 0.2291

- **Decision Tree Regression**:
  - Mean Absolute Error: 0.0791

## Tools and Technologies
- **Python Libraries**:
  - `pandas`, `numpy` for data manipulation.
  - `matplotlib`, `seaborn` for data visualization.
  - `scikit-learn` for model implementation and evaluation.
- **Jupyter Notebook** for exploratory work.

## Project Structure
```
├── data
│   └── car_dataset.csv
├── notebooks
│   └── CarSalesPrediction.ipynb
├── README.md
```

## How to Run
1. Clone the repository:
   ```bash
   git clone (https://github.com/abdelrahman-ehab/car-price-prediction)
   ```

3. Run the Jupyter notebooks in the `notebooks` folder for EDA and model building.

## Key Learnings
- Preprocessing steps like handling missing values, scaling, and encoding significantly impact model performance.
- Decision Tree models can outperform linear models like Elastic Net when the data has non-linear relationships.

## Future Improvements
- Perform hyperparameter tuning for both models to optimize performance.
- Try other advanced models such as Random Forest, Gradient Boosting, or XGBoost.
- Incorporate additional domain knowledge into feature engineering.

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests to enhance the project.




