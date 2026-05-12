# 📊 Order Analysis & Delivery Performance Dashboard (Power BI)

## 📌 Overview

This dashboard analyzes order flow, delivery timing, and delay tracking across companies and buyers.

It focuses on:

- Order execution efficiency
- Delivery delays
- Order scheduling vs reality
- Buyer & company-level order behavior

👉 Designed for operations, logistics, and sales teams to monitor execution quality.

---

# 🎯 Key Objectives

- Identify delayed orders
- Track order lifecycle (Order → Activation)
- Monitor monthly order trends
- Evaluate company & buyer performance
- Improve delivery discipline and planning

---

# 📊 Dashboard Structure

## 1. 📅 Order Timing & Delay Tracking (Company Level)

### Includes

- Company KA/PH view
- Last Order Date
- Chain Order Schedule
- Expected Next Order Date
- Order Status (Delayed / On Time)
- Days Late

### 👉 Insight

- Detect which companies are not ordering on time
- Monitor execution discipline

---

## 2. 👤 Buyer Order Delay Analysis

Same structure but at buyer level.

### Includes

- Individual buyers
- Order schedule (e.g., monthly)
- Delay status

### 👉 Insight

- Identify problematic buyers
- Detect patterns in delays

---

## 3. 📈 Monthly Order Trends

### Chart

- Order Amount vs Order Quantity

### Shows

- Monthly order value
- Monthly volume

### 👉 Insight

- Understand seasonality
- Detect drop or spike in demand

---

## 4. 🏢 Company Order Performance Table

### Includes

- Order Amount
- Order Quantity
- Sales by Activation Date
- Order Date vs Activation Date

### 👉 Insight

- Measure order processing speed
- Compare sales vs actual activation timing

---

# 🎛️ Filters (Slicers)

- Brand
- Company
- Product
- Month
- Year
- Quarter

👉 Fully dynamic filtering across all visuals.

---

# 🧠 Business Value

This dashboard helps to:

- ⏱️ Monitor order delays in real-time
- 📦 Improve supply chain execution
- 📉 Reduce late deliveries
- 👤 Identify low-discipline buyers
- 🏢 Track company-level performance
- 📅 Align ordering schedules with reality

---

# ⚙️ Logic Behind Key Metrics

## 🔴 Order Status

- **Delayed** → Order not placed on expected schedule
- **On Time** → Order follows defined schedule

---

## ⏳ Days Late

```DAX
Days Late = Today() – Expected Next Order Date
