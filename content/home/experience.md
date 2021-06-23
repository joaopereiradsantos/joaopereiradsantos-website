---
# An instance of the Experience widget.
# Documentation: https://sourcethemes.com/academic/docs/page-builder/
widget: experience
# Activate this widget? true/false
active: true
# This file represents a page section.
headless: true
# Order that this section appears on the page.
weight: 30

title: Experience
subtitle:
# Date format
#   Refer to https://sourcethemes.com/academic/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` blocks below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   You can begin a multiline `description` using YAML's `|-`.
experience:
- company: Amazon
  company_url: "https://amazon.com/"
  date_end:
  date_start: "2021-02-08"
  description: |-
   **Placement Impact Calculator & Algorithm:**
    - Collaboration with the EU FC Launch SC Team on developing a heuristic approach and tool that can be accessed via a web interface to optimize secondary transfers. The user can input a source FC, ASIN, number of units to transfer and a destination FC (optional). The algorithm would quantify the impact on placement (Local-In-Stock (LIS) as a proxy metric) of a manual transfer and optimize it. The accuracy (F1-score) of the algorithm will be determined by how accurately we can forecast LIS offending units at an FC level for the next week versus preexisting models: Availability Transfers Logic (ATS) & ML Model (Decision Tree);
    - Expected yearly savings of $ 1.25MM in transfer costs;
    - End to end algorithm and automation with SQL Extract Jobs and AWS: EC2, SageMaker and Web Application Deployment with Elastic Beanstalk.

    **Why Spread is Biased & How to Overcome it: Spread Bias:**
    - Development of a new metric: Spread Bias. A complementary metric to FC Spread (how many FCs on average an ASIN is sent to). Mathematically, it’s a weekly weighted average share of total volume cross-docked at each FC per ASIN. The more biased the volume is towards one particular FC, the more the spread bias will tend to 1. Reciprocally, the more evenly and the more FCs the volume is spread to, spread bias will tend towards 0;
    - Spread Bias is 2x more correlated to deviations in Case Break than in FC Spread. Less Spread Bias leads to a more uniform FC level placement which, in turn, increases unique inventory and reduces the risk of TRB (constraint in outbound capacity);
    - Semi-Automated Jupyter Notebook Code & Markdown paper with interactive .html python code preview and Plotly graphs, Placement Impact bridge with Pearson Correlation Analysis and SQL script for production use.

    **ITS 2% Rule & Impact on Placement:**
    - Understanding of hard constrains in optimization models (SCOT heuristic approach to reduce latency of the request easing the algorithm decision time by removing the possibility of case break) and impact on placement and financial outcomes (spread, item selection, period 1/ period 2 AR share and misplacement volume);
    - Expected a yearly decrease of 4MM units in total cross-border fulfillment (CBF) by reduction in misplaced volume, 3x more item selection leading to higher LIS, higher inventory turns and 2x less Spread Bias;
    - Semi-Automated Jupyter Notebook Code & Markdown paper with interactive .html python code preview and interactive Plotly graphs.    

    **Tote Utilization Dashboard:**
    - Tote Utilization dashboard and monitoring for the IXD Sr. Ops Managers & Area Managers. Aimed at knowledge sharing and improved users tote filling best practices in order to increase truck fill rate and tote optimization;
    - Expected an increase of 2% in the weekly average tote utilization by IXD, leading to a yearly reduction of 1.5MM totes, 1k trucks, 800 tonnes of CO<sub>2</sub> emissions and $ 1MM in overall savings;
    - Data Pipeline between 2 AWS RedShift Clusters, Daily Maintenance of 6 Tables with SQL ETL Manager and AWS QuickSight.       

    **Arc Bin Level Forecast:**
    - Improved accuracy on the arc bin level forecast with univariate multi forecasting time series using Exponential Moving Average (EMA), Auto-ARIMA and FBProphet models. QuickSight analysis and Dashboard for the preceding weekly arc bin volume and share;
    - 5% increase in forecast accuracy leading to an expected optimization in bin level planning for bin fullness balance and IXD bin offsets;
    - AWS SageMaker with Python: Pandas, Matplotlib, NumPy, Pmdarima and FBProphet, AWS RedShift and AWS QuickSight.        

    **Centralized Fluid Loading Dashboard:**
    - Centralized Fluid Loading (FL) Dashboard for the overall Productivity (fluid loading share, volume, fill rate and labor) Sustainability (saved number of trucks, CO2 emissions, plastic waste) and Savings (transportation, productivity gain, unloading cost) metrics;
    - EU IXD Fluid Loading is 100% more productive than normal pallet building and loading, loads 100% more items and reduces 50% of the trucks hence saving 13.5k tonnes of CO2 emissions;
    - SQL Scheduled Extract Jobs and Microsoft Power BI: Waffle chart, Sankey diagram & Radar chart.    

    **Sort Share and Impact on Item Selection:**
    - Deep dive analysis regarding the impact on the unique item selection based on the IXD sort share deviation to ideals. Financial outcome based on the country level Cross-Border Fulfillment (CBF) cost on different ITS algorithm decisions;
    - Improved sort share bridge to item selection and weekly WBR review in sort share deviation to ideals, right sortation and CBF due to wrong sortation;
    - SQL Extract Jobs and Statistical Analysis with Excel: Pearson Correlation Coefficient, P-Value and Linear Regression.

  location: Luxembourg, Luxembourg
  title: Business Intelligence Intern | Transportation & Supply Chain (EU IXD)

- company: Amkor Technology
  company_url: "https://amkor.com/"
  date_end: "2021-01-11"
  date_start: "2020-09-01"
  description: |-
    **Requests Management Workflow Automation & Optimization:**
    - Applied DMAIC methodology (Define, Measure, Analyze, Improve, and Control) as a data-driven improvement cycle to clearly articulate the business problem, goal, potential resources, project scope, and high-level project timeline. Aimed at improving the Request Scheduling Efficiency by over 48% in a year;
    - Implemented and Tracked KPIs with Python: Pandas, Statsmodels, Seaborn and Plotly;
    - Semi-Automated a Relative Job Prioritization System with Excel: Power Query and VBA;
    - Dashboard Prototype with Python: Dash and User Adoption with a Macro-Enabled Workbook.
  location: Mindelo, Portugal
  title: Data Analyst Intern | Physical Failure Analysis & Reliability Lab

- company: Amkor Technology
  company_url: "https://amkor.com/"
  date_end: "2020-08-01"
  date_start: "2020-02-01"
  description: |-
    **Qualitative and Quantitative Statistical Analysis in Copper Electroplating Baths:**
    - Applying linear regression and correlation models (Pearson and Spearman) with R, Minitab and Excel, easing the decision-making process associated with the control of the main chemical components concentrations and total organic contaminations (TOC);
    - Extract, Transform and Load (ETL) process applied to past manufacturing datasets, implemented on the Business Intelligence and Analytics software platform Microsoft Power BI, retrieving valuable insights.
  location: Mindelo, Portugal
  title: Master Thesis Project | Process Engineer


- company: Continental
  company_url: "https://www.continental.com/"
  date_end: "2019-09-01"
  date_start: "2019-08-01"
  description: Antifoaming Agent Study for Process Optimization in DIP Content Tire Textile Reinforcement.
  location: Lousado, Portugal
  title: Summer Research Intern

---
