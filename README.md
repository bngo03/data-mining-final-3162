# Analyzing Mutual Funds and ETFs for Investment Decisions

**Contributors**: Brandon Ngo, Joshua Sanderson  
**Course**: Data Mining — Spring 2025  
**Institution**: UNC Charlotte  
**Repository**: [GitHub Link](https://github.com/bngo03/data-mining-final-3162)

---

## Overview

This project presents a data-driven evaluation of mutual funds and exchange-traded funds (ETFs), aimed at identifying investment vehicles that provide superior risk-adjusted returns. By combining financial theory with machine learning techniques, we analyze over 24,000 funds using the **“Mutual Funds and ETFs”** dataset by Stefano Leone (Kaggle). Our analysis focuses on:

- Cost efficiency (e.g., expense ratios)
- Risk profiles (e.g., beta, Sharpe ratio)
- Performance consistency (e.g., 5-year and 10-year returns)
- Strategic management (active vs. passive)

Our objective is to support informed decision-making for both retail and institutional investors by offering intuitive visualizations and empirically grounded insights.

---

## Dataset Summary

**Source**: Kaggle — [Mutual Funds and ETFs Dataset by Stefano Leone](https://www.kaggle.com/datasets/stefanoleone992/mutual-funds-and-etfs)  
**Size**: 24.8 MB  
**Observations**: 24,239 funds  
**Features**: 27  

### Key Variables:
- **Fund Attributes**: Name, category, inception date, fund family, strategy (active/passive)
- **Performance Metrics**: Annual returns (1Y, 3Y, 5Y, 10Y), dividend yield, NAV
- **Risk Indicators**: Beta, alpha, standard deviation, Sharpe ratio, Morningstar rating
- **Cost Metrics**: Expense ratio, management and load fees
- **Operational Characteristics**: Turnover ratio, total net assets, minimum investment

---

## Methodology

We employed the following techniques to derive actionable insights:

### 📈 Linear Regression
Used to assess the relationship between:
- Expense ratios and long-term returns
- Risk metrics (e.g., beta) and return variability

We specifically tested the hypothesis that passively managed ETFs with lower expense ratios outperform actively managed mutual funds on a risk-adjusted basis.

### 🤖 K-Means Clustering
Funds were grouped based on:
- 5-year returns
- Expense ratios
- Sharpe ratios
- Total net assets

Clusters were assigned performance ratings (A+ to F) to facilitate fund comparison by peer group.

### 🔍 Comparative Analysis
Analyzed:
- Actively vs. passively managed strategies
- Top-performing funds within key asset classes (e.g., large-cap equity, bond)
- The impact of cost and turnover on returns

---

## Visual Analytics

The following visualizations support our analysis:

- **Risk vs. Return Scatter Plot** (Beta vs. 5-Year Return)
- **Bar Chart**: Average Expense Ratio by Fund Type
- **Histogram**: Distribution of 5-Year Returns
- **Box Plot**: Sharpe Ratios by Fund Category
- **Correlation Heatmap**: Key financial variables

All outputs are located in the `/visuals/` directory.

---

## Evaluation Plan

To validate our methodology and findings, we conducted a peer review with finance students and assessed:
- Clarity of visualizations and insights
- Usability of models for selecting funds by risk tolerance
- Effectiveness of grading via clustering

### Metrics:
- Regression performance: R², RMSE, p-values
- Clustering validation: Silhouette score
- Qualitative feedback from survey respondents

---

## Project Timeline

| Task | Deadline | Responsibility |
|------|----------|----------------|
| Data Preprocessing | April 22 | Brandon & Joshua |
| Regression Modeling | April 25 | Brandon & Joshua |
| Clustering Analysis | April 28 | Brandon & Joshua |
| Insights & Conclusion | April 30 | Brandon & Joshua |
| Impact Analysis | May 3 | Brandon & Joshua |
| Presentation Materials | May 5 | Brandon & Joshua |
| Final Code Upload | May 8 | Brandon & Joshua |

---

## Ethical Considerations

While historical data enables predictive modeling, past performance does not guarantee future results. Investors should consider personal goals, market volatility, and economic conditions before acting on any insights derived herein.
