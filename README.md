
# Fastag Fraud Records Analysis

## Overview
This repository contains a Jupyter Notebook that provides a comprehensive analysis of Fastag fraud data. The Fastag system is an electronic toll collection system in India, and the dataset includes transaction details, vehicle information, geographical location, and transaction amounts. The primary goal is to develop a system to detect fraudulent transactions using machine learning techniques.

## Dataset
The dataset comprises transaction records from the Fastag system with the following features:

- **Transaction_ID**: Unique identifier for each transaction.
- **Timestamp**: Date and time of the transaction.
- **Vehicle_Type**: Type of vehicle involved in the transaction.
- **FastagID**: Unique identifier for Fastag.
- **TollBoothID**: Identifier for the toll booth.
- **Lane_Type**: Type of lane used for the transaction.
- **Vehicle_Dimensions**: Dimensions of the vehicle.
- **Transaction_Amount**: Amount associated with the transaction.
- **Amount_paid**: Amount paid for the transaction.
- **Geographical_Location**: Location details of the transaction.
- **Vehicle_Speed**: Speed of the vehicle during the transaction.
- **Vehicle_Plate_Number**: License plate number of the vehicle.
- **Fraud_indicator**: Binary indicator of fraudulent activity (target variable).

The dataset can be found in **Kaggle**: [Fastag Frauds Records](https://www.kaggle.com/datasets/krishujeniya/fastag-frauds-records/data) 

## Analysis and Modeling
The notebook includes the following key sections:

### 1. Data Preprocessing and Cleaning
- Handling missing values and converting data types.
- Extracting features from the timestamp and geographical location data.
- Encoding categorical variables.

### 2. Exploratory Data Analysis (EDA)
- Visualizations to understand the distribution and relationships of different features with respect to fraudulent activities.
- Correlation heatmap, time series analysis, and vehicle speed distribution analysis.

### 3. Feature Engineering
- Encoding categorical variables and defining the feature set and target variable.

### 4. Model Training and Evaluation
- Training a RandomForest classifier and evaluating its performance using classification reports and confusion matrices.
- Feature importance analysis to identify significant features for fraud detection.

### 5. Visualization and Analysis
- Correlation heatmap to identify relationships between features.
- Time series analysis of daily transactions and fraudulent activities.

### 6. Modeling with Hyperparameter Tuning
- Performing hyperparameter tuning using GridSearchCV to improve model performance.

## Results
The analysis revealed several important observations:
- Certain vehicle types and lane types have a higher incidence of fraudulent transactions.
- Significant differences in transaction amounts and vehicle speeds between fraudulent and non-fraudulent transactions.
- Specific geographical locations with higher instances of fraud, indicating potential areas for targeted monitoring and intervention.
- Hyperparameter tuning improved the model's performance, demonstrating the importance of optimizing model parameters for better fraud detection.

## Conclusion
This comprehensive analysis provides valuable insights that can be used to enhance the effectiveness of fraud detection systems for the Fastag electronic toll collection system in India. Future work could involve exploring more advanced machine learning models and incorporating additional data sources for even better accuracy and detection capabilities.

## How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/debjit-mandal/fastag-fraud-analyis.git
   cd fastag-fraud-analyis
   ```

2. **Install Dependencies**:
   Ensure you have Python and Jupyter Notebook installed. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   Open the Jupyter Notebook:
   ```bash
   jupyter notebook FastagFraudAnalysis.ipynb
   ```

## Dependencies
The analysis requires the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- geopandas
- shapely

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
