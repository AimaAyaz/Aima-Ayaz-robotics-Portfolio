# NLP Final Project – NewsBot Text Classification & Summarization

## Problem
Readers face information overload with the constant stream of online news. The challenge is to design a system that can **classify news articles by topic** and **summarize them concisely**, helping users consume information more efficiently while considering ethical issues such as bias and misinformation.

## Approach
- **Dataset:** `newsbot_dataset.csv` (cleaned dataset of news articles).  
- **Model & Pipeline:**  
  - Text classification using TF‑IDF features + machine learning classifier (e.g., Logistic Regression, Naive Bayes).  
  - Sentiment analysis with VADER.  
  - Named Entity Recognition (NER) for extracting people, organizations, and places.  
  - Summarization using extractive methods.  
- **Workflow:**  
  1. **Preprocess** – Clean text, remove stopwords, tokenize.  
  2. **Classify** – Predict article category (business, tech, sports, etc.).  
  3. **Analyze** – Sentiment scoring and entity recognition.  
  4. **Summarize** – Generate concise summaries.  
  5. **Reflect** – Evaluate accuracy and ethical considerations.

## Results
- **Classification Accuracy:** ~85% on validation set.  
- **Sentiment Analysis:** Correctly identified positive/negative tone in sample articles.  
- **NER:** Extracted key entities (PERSON, ORG, GPE).  
- **Visuals:** Bar chart of top TF‑IDF terms, classification report, sample outputs for POS, sentiment, and entities.  
- **Demo:** Outputs available in `newsbot_dataset.ipynb`.

## How to Run
1. **Clone the repository** – Copy the repo from GitHub to your computer:  
   ```bash
   git clone https://github.com/AimaAyaz/Your-NLP-Repo.git
   
2. Navigate to the project folder – Move into the NLP project directory:
   cd NLP-ITAI2373

3. Install dependencies – Download required Python packages:
   pip install -r requirements.txt

4. Run the notebook – Open newsbot_dataset.ipynb in Google Colab or Jupyter Notebook and click Runtime → Run all.

5. Data Access: The dataset is included as newsbot_dataset.csv in the repo. The notebook automatically loads it.

Data Access
File: newsbot_dataset.csv (already in the repo).
Instructions:
  Notebook (newsbot_dataset.ipynb) loads the CSV directly.
  No external download required. 

Ethical Reflection
NLP systems must be designed with responsibility.
 Bias: News datasets may reflect political or cultural biases; classification must be interpreted carefully.
 Misinformation: Summarization should avoid distorting meaning or amplifying false claims.
 Transparency: Document model limitations and provide clear evaluation metrics.
 Accessibility: Summaries should be concise and readable for diverse audiences.

What I Learned
Technical: How to build a text classification and summarization pipeline using TF‑IDF, sentiment analysis, and NER.
Practical: Importance of preprocessing and evaluation metrics.
Ethical: Awareness of bias and misinformation risks in NLP applications.
Reflection: Clear documentation and modular code improved reproducibility and professional polish.
