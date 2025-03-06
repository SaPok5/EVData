# EV Charging Station Analysis

## 📌 Project Overview
This project analyzes electric vehicle (EV) data to determine optimal locations for EV charging stations across **Washington state**. The goal is to maximize accessibility, optimize infrastructure costs, and ensure equitable service across urban and rural areas.

## 🎯 Objectives
- Identify **high-demand regions** for charging stations.
- Analyze **BEV vs. PHEV distribution** to understand charging needs.
- Evaluate the **impact of utility networks** on EV adoption.
- **Predict future EV growth** and infrastructure requirements based on model year trends.

## 🗂️ Dataset
- **Source:** CleanEV.csv
- **Key Columns:** `latitude`, `longitude`, `electric_vehicle_type`, `model_year`, `electric_utility`

## 🚀 Features & Analysis
### ✅ Data Processing
- Load and clean EV data using **Pandas**.
- Store data in **PostgreSQL** for efficient querying.

### ✅ Geospatial Analysis
- Generate **EV density heatmaps** using `folium`.
- Identify **high-EV-density regions** for charging stations.

### ✅ Statistical Analysis
- **BEV vs. PHEV** distribution visualization.
- **EV growth trends** over time.
- **Electric utility impact** on charging infrastructure.

## 🛠️ Installation & Setup
### 1️⃣ Install Required Libraries
Run the following command to install dependencies:
```bash
pip install pandas psycopg2 sqlalchemy folium seaborn matplotlib
```

### 2️⃣ Configure PostgreSQL Database
Update `DB_NAME`, `DB_USER`, `DB_PASS`, `DB_HOST`, and `DB_PORT` in the notebook.

### 3️⃣ Run the Jupyter Notebook
Execute each cell in `EV_Analysis.ipynb` to process and analyze the data.

## 📊 Outputs
- **EV Density Heatmap** (Rendered inline in Jupyter Notebook)
- **EV Adoption Over Time** (Bar charts & trend analysis)
- **EV Utility Distribution** (Top utility providers serving EV users)

## 👨‍💻 Contributing
Feel free to contribute by submitting **pull requests** or reporting **issues**.

## 📜 License
This project is **open-source** and licensed under the MIT License.

---
🚗💡 **Empowering EV Infrastructure Planning Through Data!**

