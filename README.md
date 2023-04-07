# Kaggle-Toxicity-Prediction-II

1. Install the rdkit and datamol libraries.

2. Import necessary libraries such as pandas, numpy, sklearn, and os.

3. Load the training and test data from CSV files stored in Google Drive.

4. Preprocess the training and test data by splitting the Id and x columns respectively into ChemID and AssayID columns.

5. Encode the AssayID column using LabelEncoder from sklearn.preprocessing.

6. Use the datamol library to compute molecular descriptors from the ChemID column.

7. Compute additional descriptors using rdkit library.

8. Encode the AssayID column of the new dataframe using LabelEncoder.

9. Drop unnecessary columns from the new dataframe.

10. Train a voting classifier with XGBoost, LightGBM, and RandomForest classifiers.

11. Load the test data and preprocess it as done for the training data.

12. Use the trained voting classifier to make predictions on the test data.
