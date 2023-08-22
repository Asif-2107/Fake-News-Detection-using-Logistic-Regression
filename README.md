# Fake-News-Detection-using-Logistic-Regression
The provided code is a Python script that demonstrates the process of building a fake news detection model using a logistic regression classifier and visualizing the results using Seaborn scatter plots.Here's a concise description of the code:

1.Import Libraries: The code begins by importing necessary libraries such as Pandas, NumPy, regular expression (re), NLTK's stopwords, and TfidfVectorizer from scikit-learn. It also installs the NLTK library if not already installed.

2.Data Loading and Preprocessing: The code loads a CSV file named "train.csv" containing news data. It then performs basic data preprocessing steps such as combining the 'title' and 'author' columns to create a new 'News' column and filling any missing values in the dataset.

3.Text Preprocessing: The text data in the 'News' column is preprocessed using stemming and removal of stopwords. This involves converting the text to lowercase, splitting it into words, removing non-alphabetic characters, and applying stemming.

4.Data Splitting: The code splits the preprocessed data into features (X) and labels (Y) for training and testing. It then further splits the data into training and testing sets using train_test_split function, ensuring that the proportions of fake and real news are maintained in both sets.

5.Model Training and Evaluation: A logistic regression model is trained using the training data (X_train and y_train). The accuracy of the model is evaluated on both the training and testing data to measure its performance.

6.Predictive System: The script demonstrates a predictive system where a single news article is taken from the testing set, its TF-IDF values are calculated using the trained vectorizer, and the trained model predicts whether the news is fake or real.

7.Scatter Plot Visualizations: The code uses Seaborn to create scatter plot visualizations. It showcases scatter plots of TF-IDF values for specific words, a PCA scatter plot to visualize data in 2D, and a scatter plot matrix to visualize multiple pairs of features.

8.Visualization Customization: The code provides placeholders for specific words to be visualized in the scatter plots. These placeholders ('word1' and 'word2') need to be replaced with actual words from the dataset.

The script demonstrates a pipeline from data loading and preprocessing to model training and visualization, focusing on the use of TF-IDF features for text representation and the insights gained through scatter plot visualizations.
