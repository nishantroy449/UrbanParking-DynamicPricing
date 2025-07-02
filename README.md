# 🅿️ Dynamic Pricing for Urban Parking Lots  
### Capstone Project – Summer Analytics 2025  
👨‍💻 By: Nishant Roy

---

## 🚀 Project Overview

Urban parking lots often suffer from inefficient static pricing, leading to overcrowding or underutilization.  
This project simulates a **real-time dynamic pricing engine** for 14 urban parking lots, adapting prices based on:

- Demand patterns
- Traffic conditions
- Special events
- Vehicle types
- Competitor prices

Three progressively intelligent models are implemented from scratch using only **NumPy**, **Pandas**, and **Pathway**.

---

## 🧰 Tech Stack Used

- **Python** (NumPy, Pandas)
- **Pathway** (for real-time data simulation)
- **Bokeh** (for interactive real-time visualizations)
- **Google Colab** (notebook environment)
- **GitHub** (for final project documentation)

---

## 🏗️ Project Architecture & Workflow

![Architecture Diagram](assets/architecture_diagram.png)

---

## 🔎 Pricing Models

### 1️⃣ Model 1 — Baseline Linear
Price increases linearly as occupancy increases:  
\[
\text{Price}_{t+1} = \text{Price}_t + \alpha \cdot \left( \frac{\text{Occupancy}}{\text{Capacity}} \right)
\]

---

### 2️⃣ Model 2 — Demand-Based
Uses multiple real-world features to compute a normalized demand score:  
\[
\text{Demand} = \alpha \cdot \left( \frac{\text{Occupancy}}{\text{Capacity}} \right)
+ \beta \cdot \text{QueueLength}
- \gamma \cdot \text{Traffic}
+ \delta \cdot \text{SpecialDay}
+ \epsilon \cdot \text{VehicleWeight}
\]  
\[
\text{Price}_t = \text{BasePrice} \cdot \left(1 + \lambda \cdot \text{NormalizedDemand}\right)
\]

---

### 3️⃣ Model 3 — Competitive Pricing (Optional)
Adds competitor intelligence:
- Calculates distance to nearby lots using **Haversine formula**
- Adjusts price based on **competitor prices** and **current occupancy**
- Encourages rerouting when overcrowded

---

## 📊 Visualizations

- Bokeh-based **interactive line plots** for each pricing model
- Time-series behavior of real-time pricing per lot
- Smooth, explainable price transitions across the day

---

## 📁 Repository Structure
```urban-parking-dynamic-pricing/
├── README.md # Project overview and documentation
├── .gitignore # Git ignore file
├── Dynamic_Pricing_Notebook.ipynb # Main Colab notebook with all models
├── dataset.csv # Parking lot input data
└── assets/
        └── architecture_diagram.png # Visual architecture of the system
