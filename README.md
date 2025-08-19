# ESG-Financial-Risk-Detection-for-Strategic-Decision-Making

Objective

This project explores how Environmental, Social, and Governance (ESG) metrics interact with financial performance.
The goal is to detect early-warning risk signals that can impact investment decisions, client trust, and long-term business sustainability.

Data Overview

Dataset Size: 11,000+ rows, 16 columns (2020–2025)

Sources: Combined Kaggle ESG dataset + financial KPI datasets

Key Features: ESG scores, carbon emissions, board diversity, revenue growth, operating margin, and debt ratio.

Approach
1. Data Preprocessing

Cleaned missing ESG scores using regression imputation

Normalized financial metrics across industries

Merged ESG and financial data using company identifiers

2. Feature Engineering

Created Risk Index = (Debt Ratio × Carbon Intensity) / Governance Score

Built ESG trend features (3-year moving averages)

3. Modeling

Clustering (K-Means): Segmented companies into High-Risk, Moderate-Risk, and Sustainable Leaders.

Logistic Regression: Predicted probability of financial distress based on ESG scores.

Random Forest Classifier: Ranked top ESG factors impacting net profit.

4. Visualization

Power BI dashboard with:

KPI Cards: Net Profit, ESG Score, Risk Index

Heatmap: Risk concentration by industry and region

Trend Lines: ESG performance vs profitability

Results

Companies with low governance scores had 2.5× higher risk of financial instability.

High carbon emitters showed a negative 0.65 correlation with long-term profitability.

Diversity in leadership correlated with 7–9% higher revenue growth over 5 years.

Tools & Tech

Python (Pandas, Scikit-learn, Matplotlib)

SQL for data integration

Power BI for visualization

Business Impact

This project proves how integrating ESG with financial analysis can:

Help investors de-risk portfolios.

Enable consulting firms to give data-backed sustainability advice.

Support board-level decision-making on risk management.
