# 🛍️ Amazon ReviewIQ: Sentiment Analysis on E-Commerce Reviews

## 📌 Overview

**Amazon ReviewIQ** is a machine learning-powered sentiment analysis pipeline built to derive actionable insights from Amazon product reviews. It leverages advanced transformer-based models—**RoBERTa**, **LLaMA**, and **Mistral**—fine-tuned for binary sentiment classification. This project supports both customers and product managers by highlighting product satisfaction trends and enhancing feedback visibility.

---

## 📊 Project Workflow

### 1. 🗂️ Data Collection
- Scraped real-world Amazon product reviews using robust web scraping techniques.
- Extracted relevant fields: `Review Title`, `Review Text`, `Rating`, `Product Category`, and `Date`.

### 2. 🧹 Data Cleaning & Preprocessing
- Removed duplicates and handled missing/null values.
- Normalized text using:
  - Tokenization  
  - POS Tagging  
  - Lemmatization  
  - Stopword removal  
  - Lowercasing  
- Applied text standardization for consistency in model training.

### 3. 📈 Exploratory Data Analysis (EDA)
- Visualized:
  - Review rating distributions
  - Review length histograms
  - Temporal trends in sentiments
- Identified linguistic features of highly positive vs. negative reviews.

### 4. 🤖 Model Training
- Fine-tuned:
  - [`RoBERTa`](https://huggingface.co/roberta-base)  
  - [`LLaMA`](https://huggingface.co/models?search=llama)  
  - [`Mistral`](https://huggingface.co/mistralai)
- Optimized models via:
  - Learning rate tuning  
  - Batch size adjustment  
  - Early stopping  
- Trained on a balanced dataset to reduce class bias.

### 5. 🧪 Model Evaluation
| Model     | Accuracy | Precision | Recall | F1-Score |
|-----------|----------|-----------|--------|----------|
| RoBERTa   | **96.40%** | High      | High   | High     |
| LLaMA     | 94.80%   | Medium    | Medium | Medium   |
| Mistral   | 92.50%   | Medium    | High   | Medium   |

### 6. 📊 Dashboard for Insights
- Built interactive dashboards using:
  - **Tableau**
  - **Dash (Plotly)**
- Displayed:
  - Positive vs. negative review trends
  - Top review keywords by sentiment
  - Product categories with high/low satisfaction
  - Monthly review volumes

---

## ✨ Key Features

- ⚙️ **Transformer Fine-Tuning**: Customized RoBERTa, LLaMA, and Mistral for sentiment analysis.
- 📊 **Data Visualization**: Dynamic dashboard for end-user interpretation.
- ⚡ **Scalable Design**: Handles large-scale datasets with efficient preprocessing.
- 🧠 **High Accuracy**: RoBERTa model hits **96.4%** on binary sentiment classification.

---

## ✅ Conclusion

**Amazon ReviewIQ** delivers a powerful, full-stack NLP pipeline for customer review analysis. From web scraping to transformer fine-tuning to real-time visualization, the project helps:
- 📈 E-commerce managers monitor sentiment and product satisfaction.
- 🛒 Customers make better buying decisions based on collective sentiment.

> By combining modern NLP with visual analytics, this solution promotes transparency, trust, and data-driven growth in e-commerce.


