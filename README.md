# 🅿️ Dynamic Pricing for Urban Parking Lots  
### Capstone Project – Summer Analytics 2025  
👨‍💻 By: Nishant Roy

---

## 🚀 Project Overview

Urban parking spaces are scarce, and flat-rate pricing often leads to overcrowding or underutilization.  
This project simulates a real-time dynamic pricing system for 14 urban parking lots using data streams and ML logic built from scratch.

We built **three intelligent models** for dynamic pricing that adapt to:
- Real-time demand
- Environmental conditions
- Vehicle type
- Market competition

---

## 🧰 Tech Stack Used

- **Python** (Numpy, Pandas)
- **Pathway** (for real-time simulation)
- **Bokeh** (for interactive visualizations)
- **Google Colab** (execution environment)
- **GitHub** (submission & documentation)

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
