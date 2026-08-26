# 📧 Email Marketing A/B Testing & Conversion Optimisation Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=flat&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-Statistical%20Testing-8CAAE6?style=flat&logo=scipy&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard%20Ready-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Complete-2EC4B6?style=flat)
![Verdict](https://img.shields.io/badge/Verdict-Roll%20Out%20Variant%20B-success?style=flat)

*Full funnel analysis · Statistical hypothesis testing · Customer segmentation · Revenue impact quantification*

[View Notebook](#) · [Case Study PDF](#) · [PA Data Analytics](https://padataanalytics.com)

</div>

---

## 📌 Project Overview

This project evaluates whether a new email campaign variant (Variant B) significantly improved customer engagement, conversion, and revenue compared with the control (Variant A).

Using **25,000 customer records** from a 90-day email campaign, I performed data quality validation, funnel analysis, statistical hypothesis testing, customer segmentation, and revenue impact modelling.

The objective was not simply to identify which variant performed better, but to determine whether the observed differences were **statistically significant and commercially meaningful**.

## 🎯 Business Question

> **Does Variant B actually outperform Variant A, and is the improvement large enough to justify a full campaign rollout?**

## 🏆 Key Results

| Metric | Variant A | Variant B | Improvement |
|---|---:|---:|---:|
| Open Rate | 23.99% | **36.66%** | **+52.8%** |
| Click Rate | 4.24% | **10.15%** | **+139.4%** |
| Conversion Rate | 0.59% | **1.76%** | **+201.2%** |
| Revenue per Send | $4.56 | **$18.33** | **+301.9%** |
| Unsubscribe Rate | 1.50% | 1.50% | No increase |

All primary engagement and conversion improvements were statistically significant at **p < 0.0001**. :contentReference[oaicite:2]{index=2}

### 💰 Revenue Impact

The analysis estimated:

- **$344K** incremental revenue from the campaign
- **$689K/month** projected revenue uplift at full rollout
- **$8.26M/year** projected annual revenue uplift

These projections assume the campaign is scaled at the same send volume and performance observed in the experiment. :contentReference[oaicite:3]{index=3}

## 🔬 Analysis Approach

### 1. Data Quality & Validation

- Audited missing values across 17 variables
- Checked duplicate records and customer IDs
- Validated funnel logic
- Verified randomisation between control and treatment groups
- Distinguished structural from random missingness
- Applied appropriate missing-value treatments

### 2. Exploratory Data Analysis

Analyzed:

- Customer segments
- Geographic regions
- Device types
- Age groups
- Product categories
- Revenue distributions
- Variant balance

The experiment contained **12,639 Variant A records and 12,361 Variant B records**, providing a reasonably balanced test population. :contentReference[oaicite:4]{index=4}

### 3. Funnel Analysis

Built an end-to-end marketing funnel:

**Sent → Opened → Clicked → Purchased**

For each stage I calculated:

- Conversion rates
- Absolute lift
- Relative lift
- Drop-off rates
- Variant-level performance

This allowed me to identify where the treatment created the greatest improvement in the customer journey. :contentReference[oaicite:5]{index=5}

### 4. Statistical Testing

For binary marketing KPIs such as open, click and conversion rates, I used:

**Two-Proportion Z-Test**

For revenue, which was highly skewed and contained many zero values, I used:

**Mann-Whitney U Test**

with Welch's T-Test used as a validation test.

The tests consistently showed statistically significant improvements for Variant B. :contentReference[oaicite:6]{index=6}

### 5. Customer Segmentation

I compared campaign performance across:

- VIP customers
- Loyal customers
- Returning customers
- At-Risk customers
- New customers
- Mobile, desktop and tablet users
- Subject-line types
- Send-time windows

The largest conversion improvement occurred among **VIP customers**, while the At-Risk segment also showed a meaningful response to Variant B. :contentReference[oaicite:7]{index=7}

## 📊 Key Business Insights

### Variant B materially improved the entire funnel

The treatment increased:

**Open → Click → Purchase**

rather than improving only an upper-funnel engagement metric.

The conversion rate increased from **0.59% to 1.76%**, representing a **201.2% relative improvement**. :contentReference[oaicite:8]{index=8}

### Revenue efficiency improved substantially

Revenue per email send increased from **$4.56 to $18.33**, demonstrating that the improvement translated beyond engagement into commercial performance. :contentReference[oaicite:9]{index=9}

### Customer segment matters

VIP customers experienced the largest absolute conversion lift, while At-Risk customers also responded positively.

This suggests that future campaigns should combine **A/B testing with customer segmentation** rather than relying on one campaign strategy for the entire customer base. :contentReference[oaicite:10]{index=10}

### Send timing matters

Evening campaigns between **17:00–21:00** produced the strongest engagement and conversion performance in the analysis. :contentReference[oaicite:11]{index=11}

## 💡 Recommendations

Based on the analysis:

1. Roll out Variant B to the wider audience.
2. Continue monitoring conversion and revenue after rollout.
3. Prioritise VIP and Loyal customer segments.
4. Test personalised subject lines in subsequent experiments.
5. Optimise campaigns for mobile users.
6. Test send-time optimisation.
7. Build a structured experimentation roadmap for future campaigns.
8. Continue measuring revenue impact rather than relying only on open and click rates.

## 🛠️ Tools & Technologies

- **Python**
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Statistical Hypothesis Testing
- Customer Segmentation
- Revenue Impact Modelling

## 📁 Repository Structure

```text
email-ab-testing-analysis/
│
├── Email_Marketing_AB_Testing_Analysis.ipynb
├── AB_Testing_Case_Study_Patience_Anono.docx
│
├── data/
│   ├── raw/
│   └── processed/
│
├── visuals/
│   ├── funnel analysis
│   ├── significance testing
│   ├── segmentation
│   ├── revenue impact
│   └── executive dashboard
│
├── requirements.txt
└── README.md
