# IIT-G
capstone IIT-G dynamic parking pricing
# 🚗 Dynamic Pricing for Urban Parking Lots

**Capstone Project — Summer Analytics 2025**  
Conducted by: Consulting & Analytics Club × Pathway

---

## 📌 Problem Statement

Urban parking spaces are limited and in high demand. Static pricing often leads to underutilization or overcrowding.  
This project implements a **dynamic, intelligent pricing engine** for 14 real-world parking lots using:

- Real-time vehicle data
- Traffic conditions
- Queue length
- Special events
- Nearby competitor prices

---

## 🛠 Tech Stack

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| **Python**      | Core logic and modeling          |
| **Pandas**      | Data processing                  |
| **NumPy**       | Demand function computations     |
| **Bokeh**       | Real-time interactive plots      |
| **Pathway**     | Real-time data ingestion (setup-ready) |
| **Google Colab**| Cloud coding environment         |
| **GitHub**      | Project collaboration/versioning |

---

## ⚙️ Architecture Flow

```mermaid
graph LR
A[CSV Dataset] --> B[Preprocessing in Pandas]
B --> C1[Model 1: Static Pricing]
B --> C2[Model 2: Demand-Based Pricing]
B --> C3[Model 3: Competitive Pricing]
C1 --> D[Final DataFrame]
C2 --> D
C3 --> D
D --> E[Export CSV + Bokeh Visualizations]
