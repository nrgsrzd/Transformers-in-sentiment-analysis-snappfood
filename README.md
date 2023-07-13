# Transformers-in-sentiment-analysis-snappfood
This project performs sentiment analysis using Natural Language Processing techniques and the ParsBERT model to extract sentiment from user reviews of restaurants. The dataset is preprocessed, and the model is evaluated using f1-score and accuracy metrics.

# Dataset
The SnappFood dataset is included in the attachment and consists of user comments about active restaurants in this collection, each of which has been tagged as positive or negative. The dataset is in the form of a CSV file and includes the following columns:
  text: The user comment text.
  label: The sentiment label for the comment, which can be either positive or negative.


# Text Preprocessing
In this project, the following preprocessing steps were applied to clean the text data:
  1. Lowercasing: All text data was converted to lowercase using the lower() method.
  2. Removing Punctuation: Any punctuation marks in the text data were removed using the string.punctuation module from the Python standard library.
  3. Removing Stopwords: Stopwords, which are common words that do not contribute to the meaning of the text, were removed using the nltk package's stopwords module.
  4. Tokenization: The text data was tokenized into individual words using the word_tokenize() function from the nltk package.
  5. Lemmatization: The tokenized words were lemmatized using the WordNetLemmatizer() function from the nltk package, which reduces each word to its base or dictionary form.
  6. Removing Non-Alphabetic Characters: Any non-alphabetic characters in the tokenized and lemmatized text data were removed using regular expressions.

# Sentiment Analysis
For sentiment analysis on the user comments, ParsBERT is used. ParsBERT is a language model used in the field of natural language processing and it can do tasks like detecting sentiment, named entity recognition in text, etc. Among the pretrained ParsBERT models, the following model is used for this task:
HooshvareLab/bert-fa-base-uncased-sentiment-snappfood
