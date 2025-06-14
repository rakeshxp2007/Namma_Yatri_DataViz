<p align="center">
  <img src="https://github.com/user-attachments/assets/8b890102-bade-48b1-985b-9f747101d303" width="200" alt="MainLogo"/>
</p>

<h1 align="center">Namma Yatri: Data Storytelling & Visualization</h1>

<p align="center">
  🚕 Power BI | 📊 Urban Mobility Insights | 🧠 Data Science Project<br>
  <i>Post Graduate Diploma in Data Science | IIIT Bangalore</i>
</p>

---

## 🧭 Business Objective

Namma Yatri plays a pivotal role in Bengaluru’s urban transport network. With a highly dynamic operational environment, the company must continuously evolve to:

- Adapt to shifting **demand patterns**
- **Optimise ride allocations** and pricing
- Ensure **profitability**
- Deliver **exceptional customer experience**

> We applied the **5W + 5WHY Framework** to structure our problem:
> - **Who** is involved? Drivers, Riders
> - **What** is happening? Drop-offs in conversion, revenue variations, cancellations
> - **Where** is it happening? Specific zones of Bengaluru
> - **When** does it occur? Peak vs Off-peak, time slots
> - **Why** is it important? Revenue leakage, driver idling, operational inefficiency

---

## 🎯 Project Goals

- Identify peak **demand patterns**
- Uncover **factors behind cancellations** and performance drops
- Optimise **payment method preferences** and trip durations
- Enable **data-backed marketing & resource allocation**

---

## 📦 Dataset Overview

Data model includes 5 interlinked tables:
- **Trips**, **Trip_Details** – Fact tables with transactional data
- **Assembly**, **Duration**, **Payment** – Dimension tables with location, time and payment metadata

<p align="center">
  <img src="https://github.com/user-attachments/assets/21b0dc74-7310-420e-a3d5-44a6598c6e94" width="600"/>
</p>

We followed the **Pyramid Principle** for data modeling:
1. Build a fact constellation schema
2. Join dimension keys to ensure referential integrity
3. Create calculated fields (e.g., `Part_of_day`) to segment and filter analysis

---

## 🔍 Exploratory Data Analysis (EDA)

### 🚦 Demand Analysis

- ✅ **Peak demand** observed in **Afternoon (13–14 Hrs)** and **Forenoon**
- 🕓 **Night hours (0–1 AM)** show **maximum revenue/hour**

> 🔎 **Surprising Extreme**:  
> Revenue during 0–1 AM (₹45K) and 6–7 AM was far above the mean, despite lower trip volume — likely due to surge pricing and airport transfers.

> 📌 **Unknown Result**:  
> Derived a 23% cancellation rate, a figure unknown without EDA.

---

### 📍 Pickup Zone Insights

Top-performing zones:
- **Hoskote**
- **Chamrajpet**
- **Mahadevapura**

These zones showed high **trip volume**, **low cancellations**, and above-average **fare returns**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/686467a8-68db-4ab8-b2ff-6908931dd193" width="600"/>
</p>

> 🔎 **Abnormal Distribution**:  
> Certain zones like **Anekal (42.4%)**, **C V Raman Nagar (38.2%)** showed cancellation rates **way beyond the average**, driven by longer trips and low fare/km — indicative of **driver dissatisfaction**.

---

### 🧾 Payment Method Insights

<p align="center">
  <img src="https://github.com/user-attachments/assets/c3804050-a302-42a6-8a5e-45531f213cc3" width="500"/>
</p>

- **Digital Payments** dominate (76%)
- Surprisingly, **cash payments**, while only 24% in volume, contributed to **high-value rides**

> 🔎 **Surprising Comparison**:  
> Cash rides are **4× more valuable per ride** than digital ones — implying premium customers prefer cash or digital mistrust in specific rider segments.

---

### 📈 Conversion Funnel & KPI Analysis

<p align="center">
  <img src="https://github.com/user-attachments/assets/148898d1-149c-4d8a-82e7-34639da01879" width="600"/>
</p>

- Only **45% of trips** move from quote to ride — major **drop-off**
- Calculated KPIs for:
  - **Driver & Customer Cancellations**
  - **Trip Conversion %**
  - **Revenue / Trip / Zone / Hour**

> 🔎 **Significant Outlier**:  
> Some hours like **0–1 AM** showed revenue per trip **>30% above mean**, while others like **4–5 PM** had high fares but **low conversion**.

---

## 📊 Dashboard Highlights

<p align="center">
  <img src="https://github.com/user-attachments/assets/4a714e9f-6538-4520-9482-8e03acb0df54" width="600"/>
</p>

- Segment-level filtering via **parameters**
- Dynamic **zone-time revenue heatmaps**
- Tree maps and card visuals for summary KPIs

---

## 🧮 Tools & Techniques Used

| Tool         | Use Case                               |
|--------------|-----------------------------------------|
| Power BI     | Data modeling, storytelling dashboards |
| DAX          | KPIs, Conditional Filters               |
| M Language   | Time binning, logical transformations   |
| Matrix/Funnel/Tree Plots | Visualization              |

---

## ✅ Key Recommendations

### 🔧 Operational Efficiency

- 🔄 **Rebalance driver allocation** using hourly and zone-level data
- 🧠 Use **predictive assignment models** to reduce driver idle time
- 🧮 Apply **A/B testing** for ride-suggestion UX workflows

### 📣 Marketing Strategy

- 🗺️ **Hyperlocal promotions** in zones like Hoskote and Mahadevapura
- ⏰ **Time-based discounts** during underperforming fare-rich slots (e.g., 4–5 PM)
- 💳 Promote **digital payments** via cashback incentives
- 🛡️ **Driver incentive** programs to address underperformers

---

## 🎓 Academic Context

> Submitted as part of the **Post Graduate Diploma in Data Science (IIIT Bangalore)**  
> Module: *Data Visualization and Storytelling*

Used frameworks from:
- 🧩 **5W + 5WHY Analysis**
- 🔺 **Pyramid Principle** for communication
- ✍️ **Data Storytelling Patterns** for insight generation

---


## 👥 Team Details

> Group Name: **ALRR0625**  
> Team Members: **Ankit Mathur**, **Lakshmi Sagar**, **Rakesh Kumar Sahoo**, **Rohit Vashishth**

---

## 📁 Repository Structure

```bash
Namma-Yatri-CaseStudy/
├── 📊 dashboards/
│   └── Namma_Yatri_PowerBI.pbix
├── 📄 methodology/
│   └── Methodology_Report.pdf
├── 📽️ presentations/
│   ├── PPT_Technical_Leadership.pdf
│   └── PPT_Management_Leadership.pdf
├── 🖼️ assets/
│   ├── logo.png
│   ├── dashboard_preview.png
│   ├── schema.png
│   └── key_insights_graphs/
└── 📘 README.md
