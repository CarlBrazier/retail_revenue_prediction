# Retail Revenue Prediction Task (Predicting with Limited Data)
This project develops a revenue prediction model for ABC-Retail using limited transaction data to predict quarterly revenue indices. The project addresses several key challenges including small sample sizes, varying reporting periods, and the need to aggregate daily data to quarterly predictions. This information can be used by the business to focus on the metrics that most strongly influence revenue growth.

![image](https://github.com/user-attachments/assets/4b3ed551-fc47-416d-8850-4822ed1e3d5b)
### [Data Cleaning](https://github.com/YourUsername/ABC-Retail-Revenue-Prediction/blob/main/clean_data.ipynb)
- **Order Numbers Processing**: Validated and corrected sequential order data, removing invalid order numbers (decreasing values) and handling outliers in daily order differences.
- **Transaction Data Normalization**: Calculated normalized spend per user metrics and created 7-day moving averages to smooth early period noise.
- **Quarterly Mapping**: Established consistent date-to-quarter mappings and calculated period lengths to account for varying quarter durations.
- **Data Quality Handling**: Identified and handled approximately 25.5% of problematic order number sequences.

### [Feature Engineering](https://github.com/YourUsername/ABC-Retail-Revenue-Prediction/blob/main/feature_engineering.ipynb)
- **Order-based Features**: Derived metrics from order patterns including average daily orders, order growth rates, and order volatility.
- **Transaction Features**: Created user activity metrics including normalized spend, user growth, and spend volatility.
- **Period-adjusted Features**: Normalized metrics by period length to account for varying quarter durations.
- **Interaction Features**: Developed combined metrics such as orders-per-user and spend-per-order to capture relationship dynamics between different business areas.

### [Modeling Approach](https://github.com/YourUsername/ABC-Retail-Revenue-Prediction/blob/main/modelling.ipynb)
- **Model Selection**: Implemented Ridge regression to handle the small dataset (19 training observations) while preventing overfitting.
- **Time Series Considerations**: Used time series cross-validation to maintain temporal integrity in model evaluation.
- **Feature Selection**: Carefully selected a limited feature set to avoid overfitting:
  - Daily orders
  - Order volatility
  - Average normalized spend
  - Spend volatility
  - Average smoothed users
  - User growth
  - Orders per user
  - Spend per order
- **Validation Strategy**: Held out 2022 Q4 data as a final test set to evaluate model performance on unseen data.

### Performance Results
- **Cross-validation R² Scores**: [List cross-validation R² scores]
- **Training R²**: [Training R² value]
- **Training MAPE**: [Training Mean Absolute Percentage Error]
- **Test MAPE**: [Test Mean Absolute Percentage Error]

### Key Findings
- **Top Revenue Drivers**: [List the most important features]
- **Business Insights**: 
  - [First key insight]
  - [Second key insight]
  - [Third key insight]

### Methodology Details
The project addressed several challenges specific to retail revenue prediction:
- **Small Sample Size**: Used Ridge regression with regularization to prevent overfitting
- **Data Quality Issues**: Implemented robust cleaning for problematic order sequences
- **Temporal Patterns**: Preserved time series integrity throughout model development
- **Interpretability**: Selected modeling approach that provides clear feature importance

This model helps ABC-Retail understand which metrics most strongly influence their quarterly revenue, allowing for more targeted business strategies.
- Visualization Features:
  - Pie charts to analyze launch success rates based on selected criteria from dropdown menus.
  - Scatter plots to explore correlations between payload mass and other launch variables.
  - These visualizations were interactive, allowing users to select different parameters and instantly see updated results.
