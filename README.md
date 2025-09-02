# Mini-Project-2-Introduction-to-LLMs-and-Gen-AI
# 📊 Sentiment Analysis with NLP & Word Embeddings  

## 📌 Project Overview  
This project is part of **Mini Project 2: Basics of NLP – Text Cleaning & Vectorization** under *Introduction to LLMs and Generative AI*.  

The goal is to build an **AI-powered sentiment analysis pipeline** that processes customer reviews from an e-commerce platform and classifies them into **Positive, Negative, or Neutral** sentiments.  
It demonstrates **text preprocessing, vectorization (BoW, Word2Vec, GloVe)**, and prepares data for downstream machine learning models.  

---

## 🚀 Problem Statement  

A growing e-commerce platform in **electronic gadgets** faces:  
- **200% growth** in customer base (last 3 years)  
- **25% spike** in feedback volume  

Manual review is no longer feasible.  
Business challenges include:  
- Customer Churn  
- Reputation Damage  
- Financial Loss  

The company needs an **AI-driven sentiment classification system**.  

---

## 📂 Dataset  
- **Product ID** → Unique identifier for each product  
- **Product Review** → Customer feedback text  
- **Sentiment** → Positive / Negative / Neutral  
- **Size** → 1007 rows × 3 columns  

---

## 🛠️ Methodology  

### 🔹 1. Data Preprocessing  
- Removed special characters  
- Converted text to lowercase  
- Stripped extra whitespaces  
- Removed stopwords (NLTK)  
- Applied stemming (**Porter Stemmer**)  
- Applied lemmatization (**WordNet Lemmatizer**)  

### 🔹 2. Exploratory Data Analysis (EDA)  
- Sentiment distribution (class imbalance observed)  
- Word frequency visualization  

### 🔹 3. Feature Engineering & Vectorization  
- **Bag of Words (BoW)**  
- **Word2Vec** (CBOW & Skip-gram)  
- **GloVe embeddings**  

### 🔹 4. Evaluation Metrics  
- **Macro F1-Score** → balances all classes equally  
- **Per-class Precision & Recall**  
- **Confusion Matrix**  

---

## 📈 Key Insights  
- Dataset is **imbalanced** (~85% Positive reviews).  
- **Macro F1** better reflects performance than accuracy.  
- **Word embeddings (Word2Vec & GloVe)** capture semantic meaning better than BoW.  

---

## 🏗️ Tech Stack  
- **Python** (Pandas, NumPy, Scikit-learn)  
- **NLTK / Gensim** → text processing & embeddings  
- **Matplotlib / Seaborn** → visualizations  
- **Google Colab** → implementation environment  

---

## 📊 Workflow  
```mermaid
flowchart TD
    A[Raw Data] --> B[Preprocessing]
    B --> C[EDA & Visualization]
    C --> D[Vectorization]
    D --> E[Word2Vec & GloVe Embeddings]
    E --> F[Model Training & Evaluation]
    F --> G["Deployment - Future Scope"]
