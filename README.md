# Text Analytics on Spotify User Reviews

This project applies Natural Language Processing (NLP) techniques to analyze Spotify user reviews for strategic insight. The analysis involves sentiment classification, feature-specific opinion mining, topic modeling, and a business interpretation using Porter’s Five Forces framework.

---

## Project Files

| File | Description |
|------|-------------|
| `text_analytics.ipynb` | Jupyter notebook with code for text cleaning, sentiment analysis, topic modeling, and visualizations |


---

## Dataset Description

- **Source:** Spotify user reviews
- **Columns:**
  - `review` – The raw user feedback.
  - `label` – Sentiment label (`POSITIVE` or `NEGATIVE`)

The reviews cover a range of topics, including:
- App quality and performance
- Pricing and subscriptions
- Advertisements
- Technical bugs
- Comparison with competing platforms

---

## Methodology

### 1. Data Cleaning & Preprocessing
- Converted text to lowercase
- Removed special characters, links, and numbers
- Removed extra whitespace
- Created `cleaned_review` column for analysis.

### 2. Sentiment Analysis
- Used the `label` column to plot sentiment distribution
- Generated **WordClouds** for both positive and negative reviews.

### 3. Feature-Based Sentiment Analysis
Analyzed user sentiment toward key aspects:
- `price`
- `quality`
- `support`
- `service`
- `app`
- `performance`

Findings:
- `price` and `support` had more negative sentiment
- `performance` and `app` received mixed or balanced reviews.

### 4. Topic Modeling
- Applied **Latent Dirichlet Allocation (LDA)**
- Preprocessing: stopword removal, lemmatization, document-term matrix.
- Key topics identified:
  - App crashes / bugs
  - Ad interruptions
  - Subscription issues.
  - Music recommendations and variety

### 5. Visualizations
Used:
- `Matplotlib` & `Seaborn` for plotting
- `WordCloud` for visual frequency analysis
- Topic clusters and sentiment plots for intuitive presentation.

---

## Business Analysis – Porter’s Five Forces

Insights from reviews were mapped to strategic forces:

| Force | Interpretation |
|-------|----------------|
| **Threat of New Entrants** | High – Users often mention switching to Apple Music, YouTube |
| **Bargaining Power of Buyers** | High – Complaints about pricing, support, and ads |
| **Bargaining Power of Suppliers** | Moderate – Inferred through music availability discussions |
| **Threat of Substitutes** | High – Streaming alternatives are abundant |
| **Industry Rivalry** | High – Intense competition based on experience, price, and features |

---

## Summary Pipeline
   Data Collection → Cleaning → Sentiment Analysis →Feature-Based Mining → Topic Modeling → Business Insight

   
Each step provided unique insights:
- Cleaning ensured reliable analysis
- Sentiment analysis captured user mood
- Topic modeling uncovered hidden patterns
- Porter’s model linked findings to business strategy

---

## Key Insights

- A large volume of **positive reviews** reflects general satisfaction, but **negative reviews** highlight recurring frustrations with **ads**, **app performance**, and **pricing**.
- **TextBlob sentiment scoring** helped differentiate emotional tone across features.
- **LDA topic modeling** revealed specific user concerns like:
  - App crashes
  - Annoying ads
  - Subscription cost
  - Desire for more curated music suggestions.
- These findings provide clear direction for product improvement and competitive strategy.

---

## Business Value

This analysis demonstrates how companies like Spotify can:
- Use **text analytics** to monitor customer satisfaction in real-time.
- Apply **sentiment trends** to identify at-risk user groups.
- Leverage **topic clusters** to prioritize feature updates.
- Align customer voice with strategic frameworks (e.g., Porter’s Five Forces).

---

## How to Run the Notebook
###  Requirements

Install the required Python packages:

```bash
pip install pandas numpy matplotlib seaborn textblob wordcloud gensim nltk

   

