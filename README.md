🏠 House Price Prediction — Advanced Regression
A machine learning project that predicts house prices based on area-level features using Linear Regression. Built end-to-end — from raw data exploration to model evaluation.

📌 Problem Statement
Predicting house prices accurately is a critical real-world problem in real estate, banking, and urban planning. This project builds a regression model that estimates house prices based on demographic and structural features of the area.

📂 Dataset

Source: Public dataset
Records: 5,000 rows
Features: 6 columns

FeatureDescriptionAvg. Area IncomeAverage income of residents in the areaAvg. Area House AgeAverage age of houses in the areaAvg. Area Number of RoomsAverage number of rooms per houseAvg. Area Number of BedroomsAverage number of bedrooms per houseArea PopulationPopulation of the areaPriceTarget variable — house price

🔧 Tech Stack

Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn


📊 Project Workflow
1. Exploratory Data Analysis (EDA)

Checked shape, data types, null values, duplicates
Distribution plots for all features
Box plots to identify outliers

2. Outlier Removal

Used IQR method to detect and remove outliers across all numerical features
Performed two rounds — before and after IQR removal to verify clean distribution

3. Feature Encoding

Encoded the Address column (categorical) using appropriate encoding technique

4. Feature Selection

Correlation heatmap to understand feature relationships
Notable finding: Number of Rooms and Number of Bedrooms showed moderate correlation (0.47)

5. Model Building

Split data: 80% train / 20% test
Applied feature scaling using StandardScaler
Trained Linear Regression model

6. Model Evaluation
MetricTrainTestR² Score0.91150.9126RMSE100,414101,465MAE80,92181,137MSE10,083,105,98610,295,321,311
7. Visualization

Best fit line plotted for both train and test predictions vs actual prices


📈 Key Results

R² score of 0.91 on test data — model explains 91% of price variance
Near-identical train and test R² scores confirm no overfitting
Strong linear relationship between features and house prices confirmed
