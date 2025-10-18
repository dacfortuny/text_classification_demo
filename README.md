# Text Classification Demo

This repository contains a demo notebook for experimenting with **text classification** using two different approaches:

1. **Embeddings + Traditional Classifier**
   - Convert text into vector representations.
   - Split data into training and testing sets.
   - Train a classification model.
   - Evaluate performance with standard metrics.

2. **Large Language Model (LLM) Prompting**
   - Use an LLM to classify text directly via prompting.
   - Iteratively refine prompts for better results.

---

## Dataset
The demo uses the [Twitter Airline Sentiment Dataset](https://www.kaggle.com/crowdflower/twitter-airline-sentiment) (`Tweets.csv`).
It contains tweets about US airlines labeled as **positive, neutral, or negative** sentiment.

The notebook attempts to load the dataset from:
- The local data folder (if available), or
- Downloads it automatically from Kaggle.

---

## Requirements

To create a virtual environment you’ll need to have UV installed and run:

```uv sync```

---

## Results

- **Embeddings approach**: Uses vectorized features + traditional ML for classification.
- **LLM approach**: Demonstrates few-shot prompt engineering for text classification.
