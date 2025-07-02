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

```mermaid
flowchart TD
    A[Raw CSV Data (14 Parking Lots)] --> B[Data Preprocessing]
    B --> C1[Model 1: Linear Pricing]
    B --> C2[Model 2: Demand-Based Pricing]
    B --> C3[Model 3: Competitive Pricing]
    C1 --> D[Real-Time Simulation with Pathway]
    C2 --> D
    C3 --> D
    D --> E[Live Pricing Updates]
    D --> F[Interactive Bokeh Visualization]
