# MILEAGE PREDICTION - REGRESSION ANALYSIS

## Objective
The project aims to predict city-cycle fuel consumption (miles per gallon) using regression analysis. The dataset contains a mix of categorical and continuous attributes, which influence fuel efficiency.

## Data Source
The dataset is sourced from the YBI Foundation.

## Dataset Information
The dataset consists of 398 entries and 9 attributes:
- **mpg**: Miles per gallon (target variable)
- **cylinders**: Number of engine cylinders
- **displacement**: Engine displacement
- **horsepower**: Engine power output
- **weight**: Vehicle weight
- **acceleration**: Acceleration capability
- **model_year**: Year of the vehicle model
- **origin**: Manufacturing origin
- **name**: Vehicle name/model

## Data Preprocessing
- Checked for missing values and removed them
- Standardized numerical features using `StandardScaler`

## Data Visualization
- Pairplot and regression plots were generated using Seaborn to visualize relationships between features

## Model Training
- Features (`X`): `['displacement', 'horsepower', 'weight', 'acceleration']`
- Target (`y`): `mpg`
- Train-test split: 70% training, 30% testing
- Model: **Linear Regression**

## Model Performance
Metrics calculated on test data:
- **Mean Absolute Error (MAE)**: 3.33
- **Mean Absolute Percentage Error (MAPE)**: 14.7%
- **R-squared Score**: 70.3%

## Dependencies
Install the required libraries using:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Running the Project
1. Clone the repository:
```bash
git clone <repository-url>
```
2. Run the script:
```bash
python mileage_prediction.py
```

## Conclusion
The Linear Regression model achieved an R-squared score of 70.3%, meaning it explains 70% of the variance in mileage prediction. Further improvements can be made by feature engineering, adding more attributes, or using advanced regression techniques.

## License
This project is open-source under the MIT License.

