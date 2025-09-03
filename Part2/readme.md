# Mini Project 2 – Part 2  
### Automated News Article Categorization with NLP & ML  

---

## 📌 Business Context  
In today’s fast-moving media landscape, rapid categorization and curation are essential. With articles pouring in across diverse topics, publishers need efficient systems to get the right stories to the right audience on time—crucial for retention amid information overload.  

**Challenges:**  
- **Information Overload** – Manual tagging is impractical at scale.  
- **Timeliness** – Delays lead to outdated or misplaced content.  
- **Engagement** – Personalization & relevance are vital for user retention.  

**Case Study:**  
InfoWorld, a major publisher, handles a vast repository of articles across global affairs, entertainment, politics, business, and more. Manual categorization often causes delays and inaccuracies. To optimize this, InfoWorld aims to adopt **machine learning** for automated and accurate categorization.  

---

## 🎯 Problem Definition  
As a **data scientist** on InfoWorld’s team, the goal is to build a **predictive model** that categorizes articles automatically. This ensures:  
- Faster processing of incoming content  
- Personalized content delivery  
- Improved accuracy in tagging  

---

## 📂 Dataset Information  
- **File:** `Articles.csv`  
- **Shape:** 4076 articles × 7 features  
- **Columns:**  
  - `Date published`  
  - `Category`  
  - `Section`  
  - `Headline`  
  - `Description`  
  - `Keywords`  
  - `Article text`  

---

## 🔎 Exploratory Data Analysis (EDA)  
- No missing values found.  
- No duplicate rows.  
- **Category Distribution:**  
  - Sport (53.4%)  
  - News (39.5%)  
  - Others: Business, Politics, Entertainment, Health (remaining)  

- **Section Distribution:** Highly imbalanced across ~30+ sections, with Sport, Europe, and Football dominating.  
- Extracted **publication year** from dates for trend analysis.  

---

## 🛠️ Data Preprocessing  
1. Removal of special characters (`regex`).  
2. Lowercasing all text.  
3. Removing extra whitespace.  
4. Stopword removal (NLTK).  
5. Lemmatization (WordNet Lemmatizer).  
6. Final cleaned text stored in `final_cleaned_text`.  

---

## 🔡 Text Vectorization  
- **Count Vectorizer (BoW)** – Frequency-based representation.  
- **Word Embeddings (GloVe 100D)** – Semantic vectorization using pre-trained embeddings.  
- Custom **average vectorizer** implemented to represent documents.  

---

## 🤖 Modeling  
- **Algorithms considered:**  
  - Random Forest Classifier (baseline).  
  - GridSearchCV for hyperparameter tuning.  
- **Evaluation Metrics:**  
  - Accuracy Score  
  - Classification Report (Precision, Recall, F1)  
  - Confusion Matrix  

---

## 📦 Libraries Used  
- `pandas`, `numpy`, `matplotlib`, `seaborn` – Data handling & visualization  
- `nltk` – Stopwords, Lemmatizer  
- `re` – Regex-based cleaning  
- `sklearn` – ML models, metrics, preprocessing  
- `gensim` – Word2Vec & GloVe embeddings  

---

## 🚀 Next Steps  
- Experiment with **deep learning models** (LSTM, BERT).  
- Improve handling of **imbalanced categories**.  
- Deploy as a **real-time categorization service**.  

---

## 👩‍💻 Author  
**Adnan Parwez**  
B.Tech. Computer Science  

---

 

