# Employee Sentiment Analysis

This project analyzes employee email messages to assess sentiment, identify top-performing and at-risk employees, and predict engagement trends using NLP and machine learning.

## 📁 Project Structure
```
EmployeeSentimentProject/
├── Employee.ipynb # Main notebook with code and commentary
├── outputs/ # CSV outputs
│ ├── test_labeled.csv
│ ├── monthly_scores.csv
│ ├── top_3_positive.csv
│ ├── top_3_negative.csv
│ ├── flight_risks.csv
├── visualization/ # EDA plots
│ ├── sentiment_distribution.png
│ ├── monthly_sentiment_trend.png
│ ├── top_10_employees.png
│ ├── word_count_distribution.png
```
## ✅ Tasks Completed

### 1. Sentiment Labeling
- Used **VADER (NLP)** to classify each message as **Positive**, **Negative**, or **Neutral**
- Added sentiment label column in `test_labeled.csv`

### 2. Exploratory Data Analysis (EDA)
- Created and saved the following insights:
  - Sentiment distribution
  - Monthly sentiment trends
  - Top 10 most active employees
  - Word count distribution

### 3. Monthly Sentiment Score
- Assigned:
  - +1 → Positive
  - -1 → Negative
  - 0 → Neutral
- Aggregated by `employee` and `month` in `monthly_scores.csv`

### 4. Employee Ranking
- Extracted **Top 3 Positive** and **Top 3 Negative** employees monthly
- Saved to `top_3_positive.csv` and `top_3_negative.csv`

### 5. Flight Risk Identification
- Flagged employees who sent **≥ 4 negative messages** within any **30-day rolling window**
- Final list saved in `flight_risks.csv`

### 6. Predictive Modeling
- Built a **Linear Regression model** to predict sentiment scores using:
  - Message count
  - Average message length
- Evaluated using MSE and R²

---

## 📊 Summary Insights

- **Most Sentiment is Positive**, indicating good engagement
- **Top Contributors** are mostly from Enron
- **Flight Risks** detected via temporal patterns in negativity
- **Model predicts sentiment score reasonably well** using message stats

---

## 🚀 Deliverables

All CSVs are inside the `outputs/` folder and all EDA visuals are inside the `visualization/` folder.

---

## 👤 Author

**Kunal Vishwa Sivakumar**  
M.S. Applied Data Analytics, Boston University  

