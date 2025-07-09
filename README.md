# CAPSTONE-PROJECT
contains CAPSTONE PROJECT CODE AND README FILE submissions of the course
# Dynamic Pricing for Urban Parking Lots 🚗📊 MODEL-1 AND MODEL-2

## 📌 Overview

This project implements a **dynamic pricing model for urban parking lots** using real-time traffic data, occupancy levels, and other contextual features. The goal is to optimize parking prices to balance demand, reduce congestion, and improve utilization using a streaming data pipeline.

Built as a part of **Summer Analytics 2025 Capstone** by the Consulting & Analytics Club × Pathway.

---

## 💻 Tech Stack

| Technology | Purpose |
|-----------|---------|
| **Python** | Core programming language |
| **Pathway** | Real-time data streaming and transformation |
| **Pandas** | Data preprocessing |
| **Bokeh / Matplotlib** | Data visualization |
| **Git & GitHub** | Version control and submission |

---
## Project Workflow
1.Load & Preprocess Data
Historical parking lot data loaded using pandas.
Converted to a simulated stream with timestamps.

2.Ingest Data in Pathway
Pathway reads stream.csv using pw.io.csv.read() in static mode.
Timestamp columns are merged for time-based logic.

3.Feature Engineering
Encoded traffic, vehicle type, and special-day indicators.
Derived normalized demand score based on capacity, queue, etc.

4.Dynamic Pricing Model
UDF calculates price based on demand, traffic, and vehicle type.
Output is clamped between ₹5 and ₹20.

5.Write Output
Final table with SystemCodeNumber, Timestamp, and calculatedPrice written to output.csv.

6.Visualize
Optional visualization using Python (e.g., Matplotlib or Bokeh) for trend plots and insights.

## 🏗️ Architecture Diagram

![Architecture Diagram](images/architecture.png)

---
