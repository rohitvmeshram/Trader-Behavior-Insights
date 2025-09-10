# 📊 Trader Performance vs Market Sentiment Analysis

This project explores the relationship between **trader performance** (profit & loss) and **market sentiment** using the [Fear & Greed Index](https://alternative.me/crypto/fear-and-greed-index/) and historical trading data. By combining sentiment classification with execution-level trading data, we analyze how sentiment regimes (*Extreme Fear, Fear, Neutral, Greed, Extreme Greed*) impact trader profitability and activity.

---

## 📂 Project Structure

├── Untitled37.ipynb # Main Jupyter Notebook with full code
├── fear_greed_index.csv # Sentiment dataset
├── historical_data.csv # Trader execution dataset
├── README.md # Project documentation
└── outputs/ # Saved plots & result tables

---

## 🚀 Objectives

- Understand how market sentiment influences trader performance.  
- Quantify differences in profit/loss across sentiment regimes.  
- Provide actionable recommendations for sentiment-aware trading strategies.  

---

## 🛠️ Methodology

1. **Data Loading & Cleaning**  
   - Loaded CSV files (`fear_greed_index.csv`, `historical_data.csv`).  
   - Parsed dates, converted numeric fields, handled missing values.  

2. **Feature Engineering**  
   - Mapped each trade to the closest sentiment index date.  
   - Created a merged dataset with `Closed PnL` and sentiment classification.  

3. **Exploratory Data Analysis (EDA)**  
   - Summary statistics of sentiment index and trade performance.  
   - Trade counts and PnL distributions across sentiment categories.  

4. **Visualizations**  
   - 📈 Fear & Greed Index over time  
   - 📦 Boxplot of Closed PnL by sentiment  
   - 🔵 Scatter plot of PnL vs sentiment index value  
   - 📊 Bar chart of trade volume per sentiment category  

5. **Statistical Testing**  
   - Correlation between sentiment index and Closed PnL  
   - T-test comparing Fear vs Greed regimes  

6. **Insights & Recommendations**  
   - Summarized findings and strategy implications  

---

## 📈 Key Results

- Traders achieved **higher average profits** during *Greed* and *Extreme Greed* regimes.  
- The majority of trades occurred during *Fear* and *Neutral* periods.  
- Weak correlation between sentiment index and PnL → sentiment alone does not drive profitability.  
- T-test indicates a **statistically significant** difference in PnL between Fear and Greed.  

---

## 🔑 Conclusions

- Market sentiment has measurable effects on trader outcomes.  
- Greed regimes provide higher profit opportunities but come with higher volatility.  
- Extreme Fear can signal potential undervaluation and entry opportunities.  
- Best practice: combine sentiment with **trend, volume, and fundamentals** for robust strategies.  

---

## 📦 Outputs

- **Plots** (exported from notebook):  
  - Sentiment index over time  
  - Closed PnL by sentiment  
  - PnL vs sentiment scatter  
  - Trade volume by sentiment  

- **Tables**:  
  - Summary statistics per sentiment regime  
  - Average PnL by sentiment  
  - T-test results  

---

## ⚡ How to Run

1. Clone this repo or download the files.  
2. Open the notebook in **Google Colab** or **Jupyter Notebook**.  
3. Upload `fear_greed_index.csv` and `historical_data.csv`.  
4. Run all cells to reproduce the analysis.  

```bash
# Install dependencies if needed
pip install pandas numpy matplotlib seaborn scipy
