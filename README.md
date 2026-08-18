# A/B Test Analysis: Landing Page Optimization

## 📊 Project Overview
Statistical analysis of an A/B experiment comparing two landing page versions 
(A and B) for an e-commerce platform. The goal was to determine which version 
performs better in terms of conversion rate and average revenue per user, in 
order to support a data-driven business decision.

## 🎯 Business Questions
- Is there a significant difference in average spend between page A and page B?
- Which page generates a higher conversion rate?
- Does conversion depend on traffic source or user type?

## 🧪 Methodology
1. **Data validation** — checked for duplicates, nulls, and correct data types
2. **Welch's t-test** — compared average spend between converted users, after 
   validating variance equality with **Levene's test**
3. **Z-test for proportions** — compared conversion rates between page A and B
4. **Chi-square test of independence** — evaluated association between 
   conversion and traffic source / user type
5. **Data visualization** — grouped and stacked bar charts (seaborn/matplotlib) 
   to support statistical findings

## 🔑 Key Findings
- **Page B outperforms Page A** in both conversion rate (15.96% vs 12.57%) 
  and average spend ($68.75 vs $61.09 per converted user)
- Traffic source shows a **weak but statistically significant** association 
  with conversion (p = 0.034)
- User type (new vs. returning) shows **no significant association** with 
  conversion (p = 0.474)

## 💡 Business Recommendation
Implement **Page B** as the definitive landing page version, based on 
consistent statistical evidence across both conversion rate and revenue 
metrics.

## 🛠️ Tools & Libraries
Python · pandas · scipy.stats · statsmodels · seaborn · matplotlib

## 📁 Repository Structure
