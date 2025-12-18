# Sentiment Analysis on Amazon Reviews

This project demonstrates sentiment analysis on Amazon product reviews using multiple Natural Language Processing (NLP) techniques in Python.

## Overview

The notebook compares three different approaches to sentiment analysis: 

1. **VADER (Valence Aware Dictionary and sEntiment Reasoner)** - A bag-of-words approach that uses a lexicon-based method to score sentiment
2. **RoBERTa Pretrained Model** - A transformer-based model from Hugging Face that considers word context for more nuanced sentiment understanding
3. **Hugging Face Pipeline** - A simplified interface for applying pre-trained sentiment models

## Dataset

The project uses the **Amazon Fine Food Reviews** dataset from Kaggle, containing product reviews with ratings from 1-5 stars.  The analysis is performed on the first 500 reviews for demonstration purposes.

## Key Features

- **Data Visualization**: Bar plots showing the distribution of review scores and sentiment metrics
- **NLTK Integration**: Natural Language Toolkit for tokenization, POS tagging, and named entity recognition
- **Model Comparison**: Side-by-side comparison of VADER and RoBERTa sentiment scores
- **Detailed Analysis**: Pairplot visualization comparing sentiment scores across different review ratings
- **Edge Case Examples**: Identifies and analyzes reviews where sentiment models and star ratings diverge (e.g., positive sentiment in 1-star reviews, negative sentiment in 5-star reviews)

## Results

The notebook demonstrates how different models handle sentiment analysis:
- **VADER** is fast and works well for social media text
- **RoBERTa** provides more sophisticated context-aware sentiment scoring
- Comparison reveals interesting cases where automated sentiment scores don't match the user's star rating

## Requirements

- pandas, numpy
- matplotlib, seaborn
- nltk
- transformers
- scipy
- kagglehub

## Usage

Run the notebook in Google Colab or locally with Jupyter to perform sentiment analysis on Amazon reviews and compare the different NLP techniques.
