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
- Text preprocessing and tokenization using `CountVectorize` with stop_word='english' to filtering the stopword. It builds a dictionary of features and transform texts to feature vectors.
- Data transforming using `TF-IDF`.
- Model Training using `LogisticRegression`.
- Model Evaluation using `Cross Validation`.

