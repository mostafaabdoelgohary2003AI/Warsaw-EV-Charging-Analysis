# Warsaw EV Charging Analysis

## Project Overview

This project provides a comprehensive analysis of Warsaw's electric vehicle (EV) charging infrastructure, examining business performance, geographic patterns, customer behavior, and future demand forecasting. The analysis uses four datasets covering 114,000+ charging sessions across 67 stations and 8,000+ customers in 18 Warsaw districts.

## 📊 Datasets

The analysis combines four CSV datasets:

1. **charging_sessions.csv** (~114,000 records)
   - Session IDs, customer IDs, station IDs
   - Timestamps, energy charged (kWh)
   - Cost per kWh and total costs

2. **charging_stations.csv** (67 stations)
   - Station locations (latitude, longitude)
   - District assignments, income tiers
   - Operators and plug counts

3. **customers.csv** (~8,000 customers)
   - Customer IDs, income tiers
   - Car models and battery capacities

4. **districts.csv** (18 districts)
   - District names, income tiers
   - Projected EVs and charging infrastructure

## 🔧 Setup and Installation

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Installation

1. Clone or download this repository

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook warsaw_ev_analysis.ipynb
```

## 📈 Analysis Structure

The notebook is organized into six comprehensive sections:

### Section A: Data Loading & Quality Assessment
- Load and validate all datasets
- Data quality checks (missing values, duplicates)
- Feature engineering (time-based features, efficiency metrics)
- Dataset merging and integration

### Section B: Business & Operational Metrics
- Overall business performance (revenue, sessions, customers)
- Revenue analysis by operator, district, and station
- Station utilization rates and performance metrics
- Peak hours and day-of-week patterns
- Customer lifetime value and behavior analysis
- Customer segmentation by frequency

### Section C: Geographic & Demographic Analysis
- Income tier analysis and spending patterns
- Car model preferences and usage
- District-level supply vs. demand analysis
- Infrastructure gap identification
- Interactive geographic maps showing station locations
- Heat maps of usage intensity

### Section D: Statistical Analysis
- Correlation analysis of key variables
- Hypothesis testing:
  - Income tier effects on charging behavior (ANOVA)
  - Operator performance differences (ANOVA)
  - Weekend vs. weekday usage patterns (t-test)
- Customer segmentation using K-Means clustering
- Time series analysis of monthly trends

### Section E: Predictive Analytics
- Revenue prediction model (Linear Regression)
  - R² score and model performance metrics
  - Feature importance analysis
- Demand forecasting by district
- Infrastructure capacity recommendations
- Customer churn risk analysis
  - Churn risk categories (Active, Low, Medium, High)
  - Revenue at risk quantification

### Section F: Key Findings & Recommendations
Comprehensive summary including:
- Business performance highlights
- Geographic and infrastructure insights
- Customer behavior patterns
- Statistical findings
- Predictive insights and forecasts
- Strategic recommendations for:
  - Infrastructure expansion
  - Revenue optimization
  - Customer engagement
  - Operational efficiency
  - Data-driven decision making
- Risk assessment and mitigation strategies

## 🎯 Key Findings

### Business Performance
- Total revenue generated across all operations
- Average customer lifetime value
- Top-performing operators and districts
- Peak usage hours identified for operational planning

### Infrastructure Insights
- Identified underserved districts requiring expansion
- Calculated infrastructure gaps (projected vs. actual plugs)
- High-utilization stations flagged for capacity upgrades
- Geographic distribution analysis reveals optimization opportunities

### Customer Insights
- Customer segmentation reveals four distinct user groups
- Income tier significantly influences charging behavior
- Popular EV models identified for targeted marketing
- Churn risk analysis identifies at-risk customer segments

### Predictive Analytics
- Revenue prediction model achieves high R² score
- Forecasted demand growth by district
- Capacity expansion requirements quantified
- Customer retention opportunities identified

## 📊 Visualizations

The notebook includes 20+ interactive visualizations:
- Bar charts, line charts, and scatter plots
- Pie charts for categorical distributions
- Box plots for statistical distributions
- Correlation heatmaps
- Geographic maps (Folium and Plotly)
- Time series trend analysis
- Customer segmentation visualizations

## 🗺️ Generated Files

Running the notebook generates:
- `warsaw_stations_map.html` - Interactive map of all charging stations

## 💡 Recommendations

### Priority Actions

1. **Infrastructure Expansion**: Add charging plugs in underserved districts, prioritizing areas with highest demand-supply gaps

2. **Customer Retention**: Launch re-engagement campaigns for at-risk customers (Medium/High churn risk)

3. **Revenue Optimization**: Implement dynamic pricing during peak hours (8-18h)

4. **Geographic Rebalancing**: Redistribute capacity from overserved to underserved areas

5. **Operator Partnerships**: Expand partnerships with top-performing operators

### Strategic Initiatives

- Deploy VIP programs for power users (30+ sessions)
- Create targeted offers for occasional users to increase frequency
- Optimize maintenance schedules during low-usage hours
- Use predictive models for financial and capacity planning

## 📚 Technical Details

### Libraries Used
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn, plotly, folium
- **Machine Learning**: scikit-learn
- **Statistical Analysis**: scipy

### Analysis Techniques
- Exploratory Data Analysis (EDA)
- One-way ANOVA
- Independent t-tests
- K-Means clustering
- Linear regression
- Time series analysis

## 📝 Notes

- All monetary values are in local currency
- Time ranges reflect the dataset period (August - November)
- Projections are based on district-level EV adoption forecasts
- Model performance metrics are calculated on test data (20% holdout)

## 🔄 Future Enhancements

Potential extensions to this analysis:
- Real-time demand prediction
- Seasonal decomposition for better forecasting
- Advanced ML models (Random Forest, XGBoost)
- Customer churn prevention models
- Price elasticity analysis
- Station placement optimization algorithms

## 📧 Contact

For questions or suggestions regarding this analysis, please refer to the project documentation.

---

**Last Updated**: 2024

**Analysis Framework Version**: 1.0

**Data Coverage**: August - November 2025

