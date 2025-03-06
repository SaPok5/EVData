# EV Charging Station Analysis

## Overview
This project analyzes electric vehicle (EV) data to identify optimal locations for EV charging stations in Washington state. The analysis includes clustering, heatmap visualization, predictive modeling, and comparisons between BEVs (Battery Electric Vehicles) and PHEVs (Plug-in Hybrid Electric Vehicles). The dataset is stored and processed using PostgreSQL.

## Features
- **Database Integration**: Loads and processes data using PostgreSQL.
- **Geospatial Analysis**: Uses K-Means clustering to find optimal charging locations.
- **Heatmap Visualization**: Displays EV density across the state.
- **EV Type Comparison**: Analyzes the distribution of BEVs vs. PHEVs.
- **Growth Prediction**: Uses machine learning to predict future EV adoption trends.
- **Utility Analysis**: Examines EV distribution by electric utility provider.
- **Effectiveness Analysis**: Compares range and adoption rates of BEVs vs. PHEVs.

## Installation
### Prerequisites
- Python 3.8+
- PostgreSQL
- Required Python libraries:

```sh
pip install pandas psycopg2 sqlalchemy folium seaborn matplotlib scikit-learn
```

## Usage
### 1. Setup PostgreSQL Database
Ensure PostgreSQL is running and update the connection parameters in the script:
```python
DB_NAME = "ev_registrations"
DB_USER = "postgres"
DB_PASS = "your_password"
DB_HOST = "localhost"
DB_PORT = "5432"
```

### 2. Load Data into Database
The script loads `CleanEV.csv` into a PostgreSQL table named `ev_data`.
```sh
python ev_analysis.py
```

### 3. Run Analysis
The script performs:
- EV heatmap visualization
- K-Means clustering for charging station optimization
- EV growth predictions
- Distribution analysis by utility providers

## Results & Insights
### Key Findings
1. **High EV Density Areas**
   - Counties with highest EV adoption should prioritize charging station deployment.
2. **BEV vs. PHEV Considerations**
   - BEVs need fast chargers, while PHEVs require more Level 2 stations.
3. **Utility Providers**
   - Collaboration with top electric utilities is crucial for infrastructure scaling.
4. **Future EV Growth**
   - EV adoption is projected to grow 20-30% annually.
5. **Equity in Charging Access**
   - Rural areas require subsidized charging infrastructure.

### Recommendations
- Install fast-charging hubs in high-adoption areas.
- Expand Level 2 charging in underserved regions.
- Collaborate with utilities for power grid upgrades.
- Plan for infrastructure scaling based on predicted EV growth.

