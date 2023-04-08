# This code for developed for Kaggle-Toxicity-Prediction-II

The competition is simple: use machine learning to create a model that predicts which chemicals are toxic.

# Background
With new chemicals being synthesized every day, toxicity prediction of newly synthesized chemicals is mandatory before they could be released in the market. For a long time, *in-vivo* methods have been used for toxicity prediction which involves studying bacteria, human cells, or animals. With thousands of new chemicals being synthesized every day, it is not feasible to detect toxicity with traditional laboratory animal testing. One great alternative to *in-vivo* methods is the *in-silico* techniques that have great potential to reduce the time, cost, and animal testing involved in detecting toxicity. This dataset is prepared using a resource that has data for approximately 9,000 chemicals with more than 1500 high-throughput assay endpoints that cover a range of high-level cell responses.


# Summary of Code

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

# Getting Started

To run this code in Google Colab, follow these steps:

Open Google Colab in your web browser.

Click on "File" and then "Open Notebook".

Select the "GitHub" tab and enter the following URL: 
https://github.com/MilindRahatwal/Kaggle-Toxicity-Prediction-II/blob/main/Toxicity_Pred.ipynb

Click on the "Search" button and then click on "Toxicity_Pred.ipynb".

The notebook will now open in Google Colab.

Now download the test and train file from the repository and load it in test_df and train_df

Click on "Runtime" and then "Run all" to run the entire notebook.

After the code is executed the prediction of the file will be saved and downloaded.

Upload that file in Kaggle Toxicity Prediction II challenge to get the results. 


# Prerequisites

To run this code, you will need:

A Google account to access Google Colab.
An internet connection to download the necessary files and libraries.


