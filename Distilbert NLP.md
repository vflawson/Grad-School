# Distilbert-NLP-Sentiment-Model
Positive/negative sentiment model on cleaned text data using Distilbert NLP pre-trained model from Hugging Face

Using cleaned text data, such as scraped and cleaned comments from social media platforms (please see my other repositorities),
the pre-trained distilbert-base-uncased-finetuned-sst-2-english model from Hugging Face will label each text in terms of
positive or negative sentiment.

The model also provides a certainty score to indicate the degree to which the model is certain of that particular label.

First I define the model using the "sentiment analysis" pipeline from the Transformers package before running it on the clean text data.
