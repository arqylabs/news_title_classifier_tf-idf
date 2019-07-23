## Simple News Title Classifier using TF-IDF &amp; Logistic Regression

### Content
This repo contains:
- IPython script: `spam_classifier.ipynb`.
- List of the library need as prerequisites: `Requirements.txt`.
- Dataset: `News Title.xls` with four categories `Business, Entertainment, Medical, Technology`

### Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes:
- Clone this repo.
- Install the prerequisites.
- Run the ipython script.

### Prerequisites
- Install python
- Install `requirements.txt` using `pip`
```
pip install -r requirements.txt
```

### Data Pipeline
- Data Cleansing to remove special characters and transform the text to lowercase.
- Text preprocessing and tokenization using `CountVectorize` with stop_word='english' to filter the stopword. It builds a dictionary of features and transform texts to feature vectors. These steps to get the occurrences count of each word in the document/text.
- Data transforming using `TF-IDF`. Because of the difference in length of news titles, longer news titles will have higher average count values than shorter news titles, even though they might talk about the same topics, TF-IDF was used to populate the number of occurrences of each word in a news title by the total number of words in the news title and also for weighting it in the whole news titles that will be processed.
- Model Training using `LogisticRegression`. It used for predicting the 'Class' as it is most suitable for binary classification (after Data Transformation).
- Model Evaluation using `Cross Validation`.

