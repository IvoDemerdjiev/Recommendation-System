Recommendation System with Apache Spark and ALS
This repository contains a recommendation system implemented using Apache Spark's ALS (Alternating Least Squares) collaborative filtering algorithm. The system is designed to recommend books to users based on their historical ratings and preferences.

Overview
The recommendation system is built using the following components and steps:

Data Ingestion: The code loads two main datasets - product metadata and user ratings. The product metadata includes information about books, while the user ratings dataset contains ratings provided by users for various books.

Data Preprocessing: The code performs data preprocessing, including renaming columns, casting data types, and handling missing values.

Exploratory Data Analysis (EDA): EDA is conducted to understand the data distribution, check for null values, and analyze the rating distribution.

Feature Engineering: The code indexes categorical columns using StringIndexer and assembles them into a feature vector.

ALS Model Training: An ALS (Alternating Least Squares) collaborative filtering model is trained using the processed data. This model calculates user and product factors, which are used to make recommendations.

Model Evaluation: The code evaluates the ALS model's performance using Root Mean Square Error (RMSE).

Generating Product Vectors: The code extracts product vectors from the trained model, including factors representing the books.

Similar Product Recommendations: The code provides functions to find similar products to a given book based on cosine similarity between product vectors.

Usage
Clone this repository.

Install the required dependencies, including Apache Spark and PySpark.

Prepare your own datasets or replace the sample data files with your data. Make sure the data format and columns match the code's expectations.

Run the provided code to train the recommendation model and make recommendations.

Explore the results, including similar book recommendations.

Dependencies
Apache Spark
PySpark
Pandas
Scikit-learn
