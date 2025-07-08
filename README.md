🚗 Urban Parking Dynamic Pricing Engine
📈 Real-Time Demand-Based Pricing Simulation using Python, Pandas, NumPy & Pathway

🧠 Project Objective
This project simulates an intelligent, data-driven dynamic pricing system for 14 urban parking spaces based on real-time data streams. The goal is to:
•	Adjust parking prices dynamically based on demand, vehicle types, queue length, traffic, and special events.
•	Improve space utilization through smart pricing and rerouting logic.
•	Build all models from scratch using only Python, Pandas, NumPy, and Pathway.

🛠️ Tech Stack Used
Component	Technology
Programming	Python
Data Handling	Pandas, NumPy
Real-Time Stream	Pathway
Visualization	Bokeh
Notebook	Google Colab
Version Control	Git + GitHub





🏗️ Architecture Flow
          +---------------------------+
          |   Historical Data (CSV)   |
          +------------+--------------+
                       |
                       v
          +---------------------------+
          |     Pathway Streamer      |
          | (Ingest data with delay)  |
          +------------+--------------+
                       |
                       v
         +-----------------------------+
         | Feature Extraction in Real  |
         | Time (occupancy, traffic,   |
         | queue, events, etc.)        |
         +------------+----------------+
                      |
                      v
        +-----------------------------+
        |    Dynamic Pricing Engine   |
        |   (Models 1, 2, and 3)       |
        +------------+----------------+
                     |
                     v
         +-----------------------------+
         |   Bokeh Visualizations      |
         | (real-time pricing, etc.)   |
         +——————————————+














🧮 Pricing Models
📘 Model 1: Baseline Linear Model
•	Price updates based on previous price and occupancy:
Price_t+1 = Price_t + α * (Occupancy / Capacity)

📙 Model 2: Demand-Based Function
•	Price considers occupancy rate, queue, traffic, events, and vehicle type:
Demand = α * (Occupancy / Capacity) + β * QueueLength - γ * Traffic + δ * IsSpecialDay + ε * VehicleTypeWeight
Price_t = BasePrice * (1 + λ * NormalizedDemand)

📗 Model 3 (Optional): Competitive Pricing Model
•	Adds proximity analysis using latitude/longitude
•	Adjusts price based on nearby parking lot prices
•	Can reroute vehicles if lots are full or overpriced

📊 Visualization (using Bokeh)
•	Real-time line plots for dynamic prices of each parking space
•	Competitor price comparison charts

📂 Directory Structure
📁 Parking-Pricing-Project
│
├── 📄 README.md
├── 📄 pricing_model.ipynb       # Main Colab notebook
├── 📄 dataset.csv               # Provided dataset
├── 📁 visualizations            # Output graphs from Bokeh
├── 📁 architecture              # Architecture diagram (PNG)             


📄 Report Highlights
•	Demand Function with all feature weights
•	Assumptions used in modeling
•	Explanation of price behavior across time and models
•	Visual proofs of model logic and outputs

✅ Submission Checklist
•	Google Colab notebook (well-commented)
•	Dynamic pricing models (from scratch)
•	Real-time simulation using Pathway
•	Bokeh visualizations
•	Architecture diagram and tech stack in README
•	Report explaining demand logic and pricing flow

🧪 Evaluation
This project is simulation-based and will be evaluated on:
•	Code clarity and logic
•	Effectiveness of pricing behavior
•	Quality of visualizations
•	Real-time simulation setup
