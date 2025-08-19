# ESG-Financial-Risk-Detection-for-Strategic-Decision-Making

The Story

In 2025, investors and companies are no longer judged solely by financial metrics. Environmental, Social, and Governance (ESG) performance now directly impacts long-term profitability and reputation.

But the challenge is real: how do you quantify ESG risk alongside financial data to make smarter strategic decisions?

This project answers that question by turning ESG and financial datasets into actionable insights for companies and investors.

Understanding the Problem

Companies publish ESG scores, but these numbers rarely tell the full story.

Financial performance and ESG often move independently, making risk assessment tricky.

Decision-makers needed a way to visualize risk and detect patterns early.

The Approach

Data Collection

Combined ESG datasets with financial KPIs (2015–2025) for 11,000+ projects/companies.

Feature Engineering

Created Risk Index = (Debt Ratio × Carbon Intensity) ÷ Governance Score

Calculated 3-year moving averages to detect trends

Analysis & Modeling

Clustering (K-Means) to segment companies: High-Risk, Moderate-Risk, Sustainable Leaders

Random Forest Classifier to identify which ESG factors most influence net profit

Correlation Analysis between ESG scores and financial KPIs

Visualization

Power BI dashboard with:

Heatmaps of risk by industry and region

Trend lines showing ESG vs financial performance

KPI cards for quick decision-making

Key Insights

Low governance scores = 2.5x higher financial risk

High carbon-emitting companies tend to show negative correlation with profitability

Leadership diversity correlates with 7–9% higher revenue growth

Why This Matters

Helps investors de-risk portfolios by integrating ESG with financial metrics

Provides companies with early-warning signals for strategic decision-making

Turns raw ESG data into a business intelligence tool that influences real decisions

Tech Stack

Python (Pandas, Scikit-learn, Matplotlib)

SQL for data integration

Power BI for interactive dashboards

