# This code for developed for Kaggle-Toxicity-Prediction-II

The competition is simple: use machine learning to create a model that predicts which chemicals are toxic.

# Background
With new chemicals being synthesized every day, toxicity prediction of newly synthesized chemicals is mandatory before they could be released in the market. For a long time, *in-vivo* methods have been used for toxicity prediction which involves studying bacteria, human cells, or animals. With thousands of new chemicals being synthesized every day, it is not feasible to detect toxicity with traditional laboratory animal testing. One great alternative to *in-vivo* methods is the *in-silico* techniques that have great potential to reduce the time, cost, and animal testing involved in detecting toxicity. This dataset is prepared using a resource that has data for approximately 9,000 chemicals with more than 1500 high-throughput assay endpoints that cover a range of high-level cell responses.


# Steps to run the code

1. Install the rdkit and datamol libraries.

2. Import necessary libraries such as pandas, numpy, sklearn, and os.

3. Load the training and test data from CSV files.

4. Preprocess the training and test data by splitting the Id and x columns respectively into ChemID and AssayID columns.

5. Encode the AssayID column using LabelEncoder from sklearn.preprocessing.

6. Use the datamol library to compute molecular descriptors from the ChemID column.

7. Compute additional descriptors using rdkit library.

8. Encode the AssayID column of the new dataframe using LabelEncoder.

9. Drop unnecessary columns from the new dataframe.

10. Train a voting classifier with XGBoost, LightGBM, and RandomForest classifiers.

11. Load the test data and preprocess it as done for the training data.

12. Use the trained voting classifier to make predictions on the test data.
