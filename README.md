# Task-6-Kaiburr-Assessment

The text classification problem using scikit-learn libraries and a dataset named 'complaints.csv.' you can download the dataset from here : https://catalog.data.gov/dataset/consumer-complaint-database
Importing Libraries:
You start by importing the necessary libraries, including pandas, scikit-learn's modules, and other data visualization libraries.

Loading Data:
You read the data from a CSV file named 'complaints.csv' using pandas and store it in a DataFrame named 'df'.

Data Exploration and Cleaning:
You explore the dataset by checking its structure, summary statistics, and identifying missing values.

Data Visualization:
You create data visualizations to better understand the dataset, such as a count plot to visualize the distribution of complaints by product and a word cloud to visualize the most common words in the consumer complaint narratives.

Text Preprocessing:
You define a text preprocessing function called text_preprocessing to clean and preprocess the text data in the 'Consumer complaint narrative' column. The preprocessing steps include converting text to lowercase and removing punctuation.

Applying Text Preprocessing:
You apply the text_preprocessing function to the 'Consumer complaint narrative' column to clean and preprocess the text data. You also handle missing values by replacing them with an empty string.

Data Splitting:
You split the data into training and testing sets using scikit-learn's train_test_split function. The features (X) are the preprocessed consumer complaint narratives, and the target variable (y) is the 'Product' column.

Text Vectorization (TF-IDF):
You use scikit-learn's TfidfVectorizer to convert the text data into numerical features. This step transforms the text data into a TF-IDF matrix.

Model Training (Multinomial Naive Bayes):
You initialize and train a Multinomial Naive Bayes classifier using the TF-IDF transformed training data. The model is trained in an iterative manner, allowing you to update it with multiple batches of data.

Model Evaluation:
You make predictions on the test data using the trained classifier and calculate the accuracy of the model. Additionally, you generate a classification report to evaluate the model's performance in more detail, including precision, recall, and F1-score for each class.

Classification Algorithms:
You mention that you are using the Multinomial Naive Bayes classification algorithm for this task.
