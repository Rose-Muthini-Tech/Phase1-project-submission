**Aircraft Risk Analysis**
**Business Objective**
This project aims to help a company planning to expand into the aircraft industry by identifying low-risk aircraft models using historical aviation accident data. The goal is to support safe and informed procurement decisions based on real-world accident patterns.
Key stakeholders:
•	Head of Aviation Division – Decides which aircraft to invest in
•	Procurement Team – Informs aircraft acquisition strategy
•	Risk Management Team – Evaluates operational safety and financial risk
**Dataset Overview**
•	Source: National Transportation Safety Board (NTSB)
•	Time Span: 1962 to 2023
•	Records: 88,889 incidents
•	Columns: 31

**Data Preparation**
•	Filtered to include only accident cases
•	Focused on private and commercial aircraft (excluded military or unknown purposes)
•	Created new variable Total.Injury = sum of all injuries per incident
•	Dropped records missing Make or Model
•	Converted Event.Date to datetime format
**Analysis Strategy**
I analyzed accident patterns to identify aircraft with the lowest injury rates, 
focusing on models with a minimum of 10 recorded accidents to ensure statistical relevance.

**Visualizations**
1.	Top 10 Safest Aircraft Models
Bar chart showing models with the lowest average injury rates
2.	Total Injuries vs. Accident Count
Scatter plot illustrating injury volume against frequency of accidents
3.	Injury Trend Over Time
Line chart to detect shifts in accident/injury patterns from 1962 to 2023
**Key Findings**
•	Grumman G164B and Air Tractor AT 602 were among the safest aircraft, with less than 0.1 average injuries per accident.
•	These models had at least 10 reported accidents but consistently low injury totals.

**Tools Used**
•	Python, Pandas, NumPy – Data cleaning and aggregation
•	Matplotlib, Seaborn, Plotly – Visualizations
•	Jupyter Notebook – Analysis environment
