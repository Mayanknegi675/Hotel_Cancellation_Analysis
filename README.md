Hotel Booking Cancellation Analysis
📌 Project Overview
This project focuses on performing an Exploratory Data Analysis (EDA) on a comprehensive hospitality dataset containing 119,390 reservation records with 32 operational columns. The primary objective is to investigate the high frequency of booking cancellations, uncover the underlying factors driving customer churn, and provide data-backed recommendations to minimize revenue leakage and optimize room inventory management.

📊 Key Insights & Analytics
Based on the data profiling and visualization phase, the analysis revealed several critical operational trends:

High Baseline Churn: Out of all registered reservations, approximately 37.13% of bookings result in cancellations, representing a severe disruption to forecasting and revenue.

Hotel Type Variances: * City Hotels experience a significantly higher volume of cancellations compared to Resort Hotels.

Resort Hotels maintain a relatively stable baseline with a 27.98% cancellation rate, meaning roughly 72% of bookings successfully check out.

The "No Deposit" Loophole: Over 87.6% of the total dataset (104,641 bookings) featured a "No Deposit" policy. This lack of financial accountability serves as the leading driver for last-minute cancellations, as guests face zero penalty for canceling.

Distribution Vulnerabilities: The majority of volatile bookings originate from Online Travel Agencies (TA/TO) and feature extended lead times, giving customers a wide window to monitor price drops elsewhere and cancel fluidly.

🛠️ Tech Stack & Libraries
Language: Python

Data Manipulation: Pandas, NumPy

Data Visualization: Matplotlib, Seaborn

Environment: Jupyter Notebook

🚀 Business Recommendations to Minimize Cancellations
To mitigate revenue losses and stabilize booking pipelines, the following strategic changes are proposed:

Restructure Deposit Policies: Eliminate the universal "No Deposit" default strategy. Transition toward a Non-Refundable model or require a 1-night partial deposit for peak travel months (e.g., August) and high-volatility distribution channels (Online TAs).

Dynamic Lead Time Restrictions: Implement tiered cancellation windows. Bookings made months in advance should require stricter confirmation checkpoints or a tighter free-cancellation cutoff (e.g., up to 72 hours before arrival).

Inventory Alignment: Address the gap between reserved_room_type and assigned_room_type to prevent customer friction and forced re-bookings at check-in.

Proactive Confirmation Triggers: Leverage risk profiling features (e.g., high lead time + zero deposit) to trigger automated confirmation emails or SMS updates 7 days prior to arrival.

📂 Project Structure
```text
├── Data/
│   └── hotel_bookings.csv       # Dataset containing 119k reservation records
├── Untitled.ipynb               # Jupyter Notebook containing data cleaning, EDA, and visualizations
└── README.md                    # Project documentation ```
Future Scope
Build a Machine Learning Classification Model (e.g., Logistic Regression, Random Forest, or XGBoost) to predict the probability of a reservation status changing to is_canceled == 1.

Develop an interactive dashboard using Tableau or Power BI to monitor real-time cancellation rates across various market se
