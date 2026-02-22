# 📉 Customer Churn Analysis Dashboard

---

## ✴️ Project Overview
This project presents an end‑to‑end Customer Churn Analysis Dashboard built using SQL + Power BI to analyze customer retention, revenue impact, and behavioral risk indicators. The objective was to design a scalable data model, implement advanced DAX measures, and deliver executive‑ready insights to support churn reduction strategy and revenue protection.

---

## 🎯 Business Objectives
- Measure Churn Rate (%)  
- Identify Revenue Impact from Churned Customers  
- Detect High‑Value Customers at Risk  
- Analyze Churn Drivers (Plan Type, Region, Tenure, Support Behavior)  
- Build an interactive dashboard with tooltips and drill analysis  

---

## 📂 Dataset Structure
- `tab_customers`: Customer demographic details  
- `subscriptions`: Subscription plans and status  
- `transactions`: Revenue data  
- `support_tickets`: Customer support interactions  

---

## 🧱 Data Model Design
- Central dimension: `customers`  
- Separate fact tables (subscriptions, transactions, support_tickets)  
- Single‑direction relationships  
- No ambiguous joins  
- Clean filter propagation  

---

## 🧠 Advanced DAX Techniques Used
Since churn status and revenue existed in separate fact tables, `TREATAS()` was used with `CALCULATETABLE()` to correctly propagate churn filters across the customer dimension for accurate revenue attribution.  
- Context transformation using `ALL()`  
- Defensive logic with `SELECTEDVALUE()`  
- Safe division using `DIVIDE()`  

---

## 📊 Dashboard Pages
**1. Executive Overview**  
- Total Customers  
- Churn Rate %  
- Revenue Impact  
- Active vs Churned Comparison  
- Executive Insight Summary  

**2. Churn Drivers Analysis**  
- Churn by Plan Type  
- Churn by Region  
- Tenure Distribution  
- Support Behavior Impact  
- Behavioral Risk Indicators  

**3. Revenue Impact & High‑Value Risk**  
- Revenue Loss from Churn  
- High‑Value Customer Risk Segments  
- Revenue Concentration Analysis  
- Risk‑Based Insights  

---

## ✨ Advanced UX Features
- Report Page Tooltips (contextual churn insights)  
- Navigation buttons (multi‑page flow)  
- Clean executive layout  
- Insight text summaries per page  
- KPI integrity validation & stress testing  

---

## 🔍 Key Business Insights
- Churn rate aligns with behavioral risk signals.  
- Churned customers contribute disproportionately to revenue.  
- High‑tier plan holders show elevated churn probability.  
- Higher support ticket volume correlates with churn risk.  
- Certain regions demonstrate concentrated churn clusters.  
- High‑value customers require a targeted retention strategy.

---

## 💡 Business Recommendations
- Implement early‑warning triggers for customers with increasing support frequency.  
- Prioritize retention campaigns for high‑tier plan subscribers.  
- Introduce loyalty benefits for high‑revenue customers approaching renewal.  
- Monitor churn‑prone regions with proactive outreach.  
- Develop churn prediction scoring using behavioral signals.  
- Align customer success teams with high‑risk segments.

---

## ✅ KPI Integrity Validation
- Filter context stress testing  
- Churn filter propagation validation  
- SQL baseline reconciliation  
- Revenue aggregation verification  
- Cross‑page consistency checks  

---

## 🛠️ Tools Used
- SQL (Data Analysis & Validation)  
- Power BI Desktop  
- DAX (Advanced Filter Context Handling)  
- Data Modeling (Star Schema Principles)  

---

## 📌 Portfolio Value
This project demonstrates:
- End‑to‑end BI development  
- Strong data modeling fundamentals  
- Advanced DAX proficiency  
- Business‑driven analytical thinking  
- Executive‑ready dashboard design  
- Real‑world decision support capability  

---

>Note *For any questions or collaboration opportunities, feel free to reach out!*
