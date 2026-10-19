# Logistics Data Analysis: Advanced EDA & Performance Visualizations

**Author:** Unnati Mishra[cite: 4]  
**Role:** Logistics Data Analyst Intern[cite: 1, 4]  
**Deliverable:** Week 3 Project[cite: 1, 4]

---

## 📌 Project Overview
This repository contains the complete exploratory data analysis (EDA) and performance visualization pipeline for a multimodal enterprise logistics network[cite: 1, 4]. Using a simulated dataset of 1,200 commercial consignments across four transport modes (Road Freight, Express Air, Rail Freight, and Maritime), this project investigates key drivers of delivery lead times, shipping expenses, and transit delays[cite: 4].

---

## 📊 Summary of Operational Findings

| Transport Mode | Sample Count ($N$) | Mean Transit (Hrs) | Median Transit (Hrs) | Mean Cost ($USD) \vert{} Median Cost ($ USD) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Express Air** | 299 | 7.34 | 7.07 | $9,161.39 | $9,172.38 |
| **Road Freight** | 539 | 30.02 | 30.50 | $2,535.58 | $2,568.96 |
| **Rail Freight** | 237 | 37.29 | 35.86 | $1,650.68 | $1,553.14 |
| **Maritime** | 125 | 61.81 | 62.21 | $1,233.45 | $1,192.76 |

### Core Insights
* **Delivery Lead Time Profiles:** Express Air operates within a narrow window (5–10 hours)[cite: 4]. Road Freight demonstrates an extended right tail (15–55 hours) caused by highway transit friction and checkpoint audits[cite: 4].
* **Cost vs. Weight Scaling:** Express Air expenses increase steeply for payloads exceeding 3,000 kg[cite: 4]. For bulk consignments (> 5,000 kg), Rail Freight delivers cost predictability at a ~35% lower cost compared to Road[cite: 4].
* **Regional Bottlenecks:** East Hub (Kolkata) experiences a 9.4% delay outlier rate where dispatches exceed 55 hours, pointing to local warehouse staging delays[cite: 4].

---

## 📈 Visualizations Included
1. `vis1_transit_distribution.png`: KDE distribution comparing transit durations across transport modes[cite: 4].
2. `vis2_correlation_matrix.png`: Pearson correlation heatmap showing interactions between distance, weight, time, and cost[cite: 4].
3. `vis3_cost_vs_weight.png`: Scatter plot evaluating cost-weight scaling thresholds by modality[cite: 4].
4. `vis4_hub_delays.png`: Regional boxplot identifying delay spreads and bottleneck outliers across dispatch hubs[cite: 4].

---

## 🛠️ Tech Stack & Dependencies
* **Language:** Python 3.x[cite: 1, 4]
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`[cite: 1, 4]

```bash
pip install pandas numpy matplotlib seaborn
