# Real-estate-analysis-Linear-regression
Real Estate price prediction dataset with a total of 414 entries across 7 columns.

##Dataset Overview: 
The dataset contains a total of 414 entries across 7 columns. The target variable for prediction is the House Price column, with no null values present.

##Data Cleaning and Preprocessing:
The transaction date column was in a non-standard format, which required adjustment. We retained only the year portion, discarding the decimal component.
This resulted in a simplified year column with data from 2012 (126 entries) and 2013 (288 entries).
No outliers were detected in the house age column, indicating that this feature is uniformly distributed within a reasonable range.

##Exploratory Analysis:
A density map was created to visualize the distribution of houses across different areas, helping identify concentration zones.

##Feature Selection: 
Only relevant columns were retained to create a streamlined dataset for the machine learning model.

##Correlation Analysis:
The number of convenience stores and distance to the nearest MRT station showed a correlation of -0.61, indicating a negative relationship between the two.
Both features also had a significant correlation with house price. To avoid multicollinearity, one of these features was removed and tested in the model.
Model Training and Evaluation:

A linear regression model was built using the processed dataset, and predictions were made on the test set.
The model evaluation metrics were as follows:
Mean Absolute Error (MAE): 5.50
Mean Squared Error (MSE): 49.89
Root Mean Squared Error (RMSE): 7.06
R-squared (R²): 0.565, indicating the model explains about 56.5% of the variance in house prices.
Residual Analysis:

A residual plot was generated, showing a bell-shaped, nearly normal distribution. This suggests that the model is a good fit, with residuals evenly distributed around zero, indicating no major bias.
