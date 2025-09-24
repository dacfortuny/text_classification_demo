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
- Google Drive (if available), or  
- Downloads it automatically from Kaggle.  

---

## Requirements
To run the notebook, you’ll need:

- Python 3.8+  
- Jupyter Notebook or JupyterLab  
- Dependencies (install via `pip`):  
  ```bash
  pip install pandas scikit-learn matplotlib kagglehub openai
  ```

For Google Drive access (if running on Colab):  
```python
from google.colab import drive
```

---

## Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/text-classification-demo.git
   cd text-classification-demo
   ```

2. Open the notebook:
   ```bash
   jupyter notebook text_classification_demo.ipynb
   ```

3. Run all cells to reproduce results.

---

## Structure
- `text_classification_demo.ipynb` → Main notebook with both approaches.  
- `Tweets.csv` → Dataset (loaded automatically if not available locally).  

---

## Results
- **Embeddings approach**: Uses vectorized features + traditional ML for classification.  
- **LLM approach**: Demonstrates few-shot prompt engineering for text classification.  