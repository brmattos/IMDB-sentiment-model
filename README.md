# Twitter Sentiment Analysis Model
---

## Overview
This model performs sentiment analysis on a collection of 1,600,000 tweets, extracted using the Twitter API, implementing a machine learning model based on data from the Sentiment140 dataset. The primary goal is to classify tweets as either positive or negative, utilizing a Linear Regression Model and Natural Language Processing (NLP). The dataset is annotated such that tweets with positive sentiment are labeled as 4 (converted to 1 for this project), and tweets with negative sentiment are labeled as 0.

## Project Structure
- `model.ipynb`: Jupyter Notebook that cleans & formats the dataset, implementing the Linear Regression model for sentiment analysis
- `sentiment140.zip`: Zipped CSV file that contains the dataset (large file)

## Data Preprocessing
The collected data was processed and cleaned in the `model.ipynb` notebook.  
The steps included:
- Analyzing, observing, and formatting the dataset into a dataframe
- Cleaning the dataset to be readable and containing only necessary data for the model & context of the project
- **Stemming** the textual data using **Natural Langauge Tool Kit** (NLTK), removing all unnecessary words while reducing all words down to their root words

## Linear Regression Model
The `model.ipynb` notebook also implements the Linear Regression model:
- Converted all textual data to numerical values, using **scikit-learn**'s TfidfVectorizer
- Split the data for training and testing
- Evaluated the model's accuracy

## Result
`Training Accuracy`: 81%
`Testing Accuracy`: 78%
- The model demonstrates strong performance on both the training and testing datasets, indicating good generalization to unseen data
`Logistic Regression Effictiveness`:
- Logistic Regression, despite its simplicity, proved to be an effective method for sentiment analysis on this dataset
- It serves as a robust baseline model, offering decent accuracy and interpretability
- The model and preprocessing pipeline are efficient and scalable, capable of handling large datasets, making them suitable for real-world applications where large volumes of social media data need to be analyzed
