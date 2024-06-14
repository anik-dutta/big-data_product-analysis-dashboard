# Product Analysis

A simple dashboard for product analysis of Amazon build using Dash and PySpark. Various analyses of products can be done in that dashboard. The type of analyses that can be performed are:

1. Discount
    * Top 10 Subcategories with the Highest Average Discount Percentage
    * Top 5 Main Categories with the Highest Proportion of Discounted Products
    * Lowest Discount Percentage and Corresponding Main Category
    * Highest Discount Percentage and Corresponding Main Category
2. Price
    * Top 10 Subcategories with the Highest Average Actual Price
    * Top 5 Main Categories with the Highest Average Actual Price
    * Lowest Actual Price and Corresponding Main Category
    * Highest Actual Price and Corresponding Main Category
3. Ratings
    * Top 10 Subcategories with the Highest Average Ratings
    * Top 5 Main Categories with the Highest Average Ratings
    * Lowest Ratings and Corresponding Main Category
    * Highest Ratings and Corresponding Main Category
4. Popularity
    * Top 10 Subcategories with the Highest Count of Ratings
    * Top 5 Main Categories with the Highest Count of Ratings

Also, different types of data analyses were performed.

## Data
The dataset was taken from Kaggle.

## Create cluster using spark
Both master and worker machines should be in the same network.

1. To create and run master machine
    - Go to the bin folder of spark
    - type "spark-class org.apache.spark.deploy.master.Master" and hit enter
    - It will give you the IP port (IP:PORT) of the master machine

2. To create and run worker machines
    - Go to the bin folder of spark
    - type "spark-class org.apache.spark.deploy.worker.Worker spark://IP:PORT" and hit enter

3. To create and deploy Spark application
    - Go to the folder directory and type : "pyspark --master spark://IP:PORT"
    - Run run the python scripts "Amazon-Product-(Data-Analysis).ipynb" and "Amazon-Product-Analysis.ipynb"

* To monitor the machines go to "http://localhost:8080"
* The app is running on "http://localhost:8050/"

## Dependencies
* python 3
* Libraries used:
    - pyspark
    - dash
    - matplotlib
    - plotly
