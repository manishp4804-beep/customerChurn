# Customer Churn Analysis Dashboard

> **An interactive Power BI dashboard for analysing user churn behaviour across a music streaming platform**

---

## Student Details

| Field | Details |
|-------|---------|
| **Name** | Manish Pandey |
| **Roll Number** | 23053940 |
| **Program / Batch** | B.Tech CSE |
| **Academic Year** | 2023 – 2027 |
| **Tool** | Microsoft Power BI Desktop |

---

## Problem Statement

A music streaming platform is experiencing a churn rate of **~30.70%** — nearly 1 in 3 users discontinues their subscription. Without data-driven insight into *why* users churn, the business cannot make targeted retention decisions.

This project analyses 4,600 user records to uncover churn patterns across demographics, subscription plans, network quality, device usage, and music preferences.

---

## Objective

Design and deploy an interactive Power BI dashboard that:
- Tracks real-time KPIs: total users, churned users, active users, and churn rate
- Segments churn across multiple dimensions simultaneously
- Enables filtering by payment method for targeted analysis
- Provides actionable insight for retention and product teams

---

## Dataset

**File:** `churn_analysis_dataset.csv`

| Attribute | Details |
|-----------|---------|
| Total Records | 4,600 users |
| Churned Users | 1,412 (30.70%) |
| Active Users | 3,188 (69.30%) |
| Features | 12 columns |

### Columns

| Column | Description |
|--------|-------------|
| `user_id` | Unique user identifier |
| `gender` | Male / Female |
| `age_group` | 18-25, 26-35, 36-45, 46+ |
| `top_genre` | Rock, Pop, HipHop, Jazz, EDM, Classical |
| `subscription_plan` | Free, Premium, Family |
| `payment_method` | Auto-Debit, Card, UPI, Wallet |
| `auto_renewal_enabled` | Yes / No |
| `previous_subscription_plan` | Last plan before current |
| `device_type` | Android, iOS, Web |
| `network_type` | WiFi, 4G, 5G |
| `buffering_time_avg` | Average buffering time (seconds) |
| `is_churned` | Target variable — Yes / No |

---

## Dashboard Preview
 
![Customer Churn Analysis Dashboard](https://github.com/manishp4804-beep/customerChurn/blob/main/Customer%20Churn.png)
 
---

## Key Features

### KPI Cards
Four top-level cards give an instant platform health snapshot:
- **Total Users:** 4.6K
- **Churned Users:** 1.412K
- **Active Users:** 3K
- **Churn Rate:** 30.70%

### Payment Method Filter Panel
Interactive slicer to filter all visuals by: Auto-Debit, Card, UPI, Wallet

### Visuals Included

| Visual | Insight |
|--------|---------|
| Gender-Wise Churn (Bar) | Males: 2.0K active / 0.9K churned; Females: 1.2K / 0.5K |
| Age-Wise Churn (Bar) | Compares churn across 18-25, 26-35, 36-45, 46+ age groups |
| Churn by Device Type (Pie) | Android 33.47% · Web 33.61% · iOS 32.92% |
| Churn by Buffering Rate (Line) | QoS vs. churn correlation — lower quality = higher churn |
| Genre + Churn Rate (Combo) | User count bars + churn rate line across 6 genres |
| Churn by Network Type (Donut) | 4G users churn most (34.6%) vs. 5G (32.5%) and WiFi (32.9%) |
| Subscription Plan Movement (Table) | Churn % change: Premium −0.06 · Family +0.02 · Free +0.05 |

---

## Tech Stack

| Component | Technology |
|-----------|-----------|
| BI & Visualisation | Microsoft Power BI Desktop |
| Data Source | CSV file (4,600 records) |
| Data Transformation | Power Query Editor |
| Calculations | DAX (Data Analysis Expressions) |
| Filters | Power BI Slicers |
| Documentation | Python (ReportLab), Markdown |

---

## Unique Aspects

- **Multi-dimensional churn analysis** — 7 dimensions in a single dashboard view
- **Subscription plan delta tracking** — Churn % change from previous to current plan
- **Buffering time as a churn signal** — Bridges QoS metrics with business KPIs
- **India-centric payment context** — UPI, Wallet, Auto-Debit filters for local relevance
- **Balanced demographic coverage** — Proportional male/female representation
- **Modern dark-sidebar UI** — Follows contemporary BI dashboard design standards

---

## Future Improvements

- [ ] **Predictive ML Model** — Embed XGBoost/Logistic Regression for real-time churn probability scores
- [ ] **Live Data Refresh** — Connect to SQL Server / Azure Synapse with DirectQuery
- [ ] **Cohort Retention Analysis** — Monthly cohort charts to reveal user lifecycle patterns
- [ ] **Customer Lifetime Value (CLV)** — Prioritise retention by user value, not just churn risk
- [ ] **Mobile-Optimised Layout** — Dedicated Power BI mobile view for on-the-go stakeholders
- [ ] **Drill-Through Pages** — Segment-level sub-reports accessible by clicking data points
- [ ] **Automated Churn Alerts** — Power Automate notifications when churn crosses threshold

---

## Project Structure

```
churn-analysis-dashboard/
│
├── churn_analysis_dataset.csv         # Raw dataset (4,600 records)
├── CustomerChurnDashboard.pbix        # Power BI report file
├── dashboard_screenshot.png           # Dashboard preview image
├── README.md                          # This file
└── Churn_Analysis_Project_Documentation.pdf   # Full project documentation
```

---

## License

This project was developed for academic purposes as part of the **B.Tech CSE** curriculum.  
All data used is synthetic and intended solely for educational analysis.

---

<p align="center">Made with ❤️ by <strong>Manish Pandey</strong> · Roll No. 23053940 · B.Tech CSE</p>
