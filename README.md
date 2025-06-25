# 🌟 AI-Enhanced Amazon Product Insights Generator

This project is an end-to-end data analytics and GenAI application that explores Amazon product listings and user reviews to extract business-critical insights using a combination of data science, NLP, and generative AI.

---

## 📂 Dataset
- Source: [Kaggle - Amazon Sales Dataset](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)
- Contains over 1,000 Amazon product listings and user reviews.

### Key Features:
- `product_id`, `product_name`, `category`
- `discounted_price`, `actual_price`, `discount_percentage`
- `rating`, `rating_count`
- `review_title`, `review_content`
- `user_id`, `user_name`, `review_id`

---

## 🤖 Tech Stack
- Python 3
- pandas / numpy
- TextBlob (sentiment analysis)
- Hugging Face Inference API (GPT-2)
- requests

---

## 📊 Project Pipeline

### 1. Data Preprocessing
- Removed currency symbols and commas from `discounted_price` and `actual_price`
- Converted them to float for numerical operations

### 2. Sentiment Analysis
- Used `TextBlob` to analyze sentiment of `review_content`
- Added a new column: `sentiment_label` (positive, neutral, negative)

### 3. Category Insights
- Identified top product categories using `value_counts()`
- Enabled comparison of review sentiment by category

### 4. AI-Generated Insights
- Used Hugging Face's GPT-2 model via Inference API
- Summarized analytical findings into natural language insights

### 5. Reporting
- Generated a report file: `Amazon_Insights_Report.txt`
- Included:
  - Top Categories
  - Sentiment Distribution
  - AI-generated insights from GPT-2

## ⚡ Setup Instructions
```bash
# 1. Clone the repository
$ git clone https://github.com/yourusername/ai-amazon-insights
$ cd ai-amazon-insights

# 2. Install dependencies
$ pip install -r requirements.txt

# 3. Add your Hugging Face API key to the .env or directly in code
```

---

## 🌐 Live Preview (optional)
Want to build a Streamlit dashboard? Coming soon in `/streamlit_app.py`

---

## 📈 Potential Extensions
- Product price trend analysis
- Wordcloud of frequently used review terms
- Streamlit dashboard with filtering by category
- Comparison of sentiment by price bracket

---

## ✅ Credits
- Dataset: [Karkavelraja - Amazon Sales Dataset on Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)
- GenAI Model: Hugging Face Inference API

---

## 🚀 License
This project is licensed under the MIT License.
