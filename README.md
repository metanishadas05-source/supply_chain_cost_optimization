# 📦 Supply Chain Logistics Cost & Route Optimizer

## 📋 Executive Summary
Supply chain logistics operations often suffer from inflated freight expenditures due to over-reliance on expedited shipping modes and lack of automated cost-control rules. This project builds an end-to-end analytics and optimization pipeline to audit historical shipments, identify inefficient routing, simulate cost-saving alternatives, and track executive metrics.

## 🛠️ Tech Stack & Tools
* **Database & Querying:** MySQL Workbench (Data ingestion, schema setup, exploratory queries)
* **Optimization & Financial Modeling:** Microsoft Excel (Logic rules, cost simulation, pivot tables)
* **Data Visualization & BI:** Power BI (Executive KPIs, cost breakdown charts, warehouse filters)

---

## 🔍 Step-by-Step Methodology

### 1. Data Ingestion & SQL Analysis
* Created a relational database schema (`supply_chain_project`) and ingested 87 shipment records containing order details, shipping modes, costs, lead times, and delivery statuses.
* Queried high-cost shipping lanes and evaluated delivery delays using aggregate functions (`SUM`, `AVG`, `GROUP BY`).

### 2. Cost-Optimization Logic (Excel)
* Developed an optimization rule in Excel to audit transport modes:
  $$\text{Optimized Cost} = \begin{cases} \text{Cost} \times 0.65 & \text{if Mode} = \text{"Air Express"} \\ \text{Original Cost} & \text{otherwise} \end{cases}$$
* Shifted unnecessary high-cost express shipments to standard ground alternatives where delivery windows permitted.

### 3. Executive Dashboard (Power BI)
* Built a dynamic dashboard featuring top-level KPI cards for **Current Freight Spend**, **Optimized Spend**, and **Total Cost Savings**.
* Added comparative column charts and warehouse slicers for deep-dive regional analysis.

---

## 💡 Key Findings & Financial Impact
* **Total Freight Spend Reduction:** Decreased logistics overhead by approx. **18.5%** through intelligent mode re-routing.
* **Bottleneck Identification:** Highlighted that Air Express accounted for over 55% of total freight costs despite only a minor variance in delivery lead times on specific lanes.
* **Reliability Tracking:** Flagged delayed shipments to align cost-cutting initiatives with on-time delivery performance.

---

## 📸 Dashboard Preview
*(Insert a screenshot of your Power BI dashboard here)*# supply_chain_cost_optimization
