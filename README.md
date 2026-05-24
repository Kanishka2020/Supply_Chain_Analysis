# Supply_Chain_Analysis
End-to-End Order Fulfillment Analysis &amp; Predictive Insight

Content of the Project:

1.   Summary of the project 
2.   Business Context & Objectives
3.   Review the Data
4.   Data Analysis & Vizualization
5.   Business Key Performance Indicators (KPIs)
6.   Profitability Distribution
7.   Delay Distribution & Profit vs. Delay Days 
8.   Bottleneck Detection 
9.   Root Cause Analysis 
10.  Time-Based Delay Patterns 
11.  Machine Learning Model Results
12.  Conclusion


## 1. Summary of the project
This project presents a comprehensive analysis of the delivery operations of a global e-commerce company 
managing end-to-end order fulfillment across multiple regions.

The analysis covers 172,765 orders spanning 
January 2015 through January 2018, focusing on identifying root causes of chronic late deliveries, 
quantifying their financial impact, and establishing a data-driven framework for improvement.

## 2. Business Objectives
The company operates a global e-commerce platform selling products across categories including sporting 
goods, fitness equipment, outdoor gear, footwear, and apparel across multiple international regions.

### Core Business Problem
Actual shipping times frequently deviate from scheduled delivery windows, creating eroded customer trust, 
reduced order profitability, and an inability to make reliable commitments to buyers at point of purchase. 

## 3.   Overwiew of the Data
<img width="1623" height="583" alt="image" src="https://github.com/user-attachments/assets/827f1897-314f-43d8-b57e-9d0833331525" />

## 4.   Data Analysis & Vizualization
<img width="960" height="327" alt="image" src="https://github.com/user-attachments/assets/0088fddf-4f38-4340-a9e9-aa2713a68860" />

## 5. Business Key Performance Indicators (KPIs) 
<img width="340" height="201" alt="image" src="https://github.com/user-attachments/assets/cec31329-5106-4da4-bff7-5e991126361e" />

## 6.   Profitability Distribution

Order-level profitability was classified into three tiers based on Order Profit Per Order. While 80.7% of orders 
are profitable, the 18.7% loss-making share represents a meaningful drag that is disproportionately 
concentrated among delayed shipments.
<img width="580" height="450" alt="image" src="https://github.com/user-attachments/assets/05c2e7cc-0084-4bd8-8f7a-78bc001c1176" />

## 7.   Delay Distribution & Profit vs. Delay Days

The delay distribution shows that 31.0% of all orders arrive exactly 1 day late the single largest cohort. 
Combined, orders delayed by 1–4 days account for 54.7% of all order volume, directly mapping to the overall 
late delivery rate.
<img width="1707" height="644" alt="image" src="https://github.com/user-attachments/assets/fcb10d48-772d-4e99-8576-d4d678a38207" />

## 8. Bottleneck Distribution
Delay percentage was computed across six key operational dimensions. The charts below reveal where the 
fulfilment process breaks down most severely.

<img width="1530" height="671" alt="image" src="https://github.com/user-attachments/assets/d8a80c94-6f46-45a5-8863-3234e2857466" />

## 9. Root Cause Analysis
Central Africa was selected for deep-dive root cause analysis as the highest-delay region (58.7%). The chart 
below ranks the top 10 driver factors by delay percentage within this region.

<img width="787" height="424" alt="image" src="https://github.com/user-attachments/assets/c7410a1c-5f25-44ad-b53f-1ed58ca85876" />

## 10. Time-Based Delay Patterns

Three temporal dimensions were analysed: month of year, day of week, and hour of day. While delay rates 
are relatively stable across all dimensions (53–57%), specific peaks highlight opportunities for targeted 
capacity planning.
<img width="1733" height="548" alt="image" src="https://github.com/user-attachments/assets/e7f802b3-3587-491f-9fe7-b265c9b56746" />

## 11. Machine Learning Model Results

A supervised classification model was built to predict whether an individual order will be delivered late 
(Late_delivery_risk = 1). The pipeline included frequency encoding of categorical variables, stratified 
train/test split, SMOTE oversampling to address class imbalance and Random Forest classification.
<img width="881" height="43" alt="image" src="https://github.com/user-attachments/assets/2b1fca20-d616-49da-ac33-85c867668ea4" />

## 12. Conclusions
This analysis has surfaced a clear and urgent picture: a global e-commerce operation where the majority of orders (54.71%) fail to meet their promised delivery windows, costing $2.1M in at-risk profit and undermining customer trust at scale. 

The root causes are identifiable and addressable. Shipping mode misconfiguration (First Class at 100% late, Second Class at 79.8%) is the dominant operational failure. Payment processing friction creates a secondary bottleneck. Seasonal volume spikes are not adequately planned for. And geographic disparities, while present, are secondary to the systemic company-wide pattern. 

A Random Forest predictive model trained on readily available order features already achieves 74% accuracy in identifying at-risk orders. This is a deployable tool, not a future aspiration. 








