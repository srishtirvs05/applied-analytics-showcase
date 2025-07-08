# 🌡️ Energy Usage in the Carolinas – Summer Demand Forecasting

This project simulates a collaboration with the energy provider **eSC**, which serves parts of South Carolina and North Carolina. The objective is to understand July energy usage patterns and assess the impact of insulation, AC systems, and income levels on cooling demand.

## 🔍 Research Questions
- Does insulation type influence energy usage?
- How does AC type and cooling setpoint affect consumption?
- Is there a correlation between household income and electricity use?

## 🗂️ Data Sources
- Static house metadata: `static_house_info.parquet`
- Hourly house-level energy consumption: `2023-houseData/*.parquet`
- Hourly weather data: `weather/2023-weather-data/*.csv`
- Metadata Dictionary: `data_dictionary.csv`

## 🛠️ Methods
- Data extraction using R and `arrow`, `dplyr`, and `readr`
- Cleaned and merged weather and energy datasets for July
- Built models using:
  - Poisson Regression
  - Support Vector Machines (SVM)
  - Linear Regression
- Created a [Shiny App](http://127.0.0.1:6872) for interactive exploration (local only)

## 📈 Key Insights
- Cooling energy consumption increases with temperature (r = 0.64)
- Ceiling insulation and ducted AC systems show strong correlation with energy use
- Income showed minor impact in linear modeling

## 💡 Recommendations
- Incentivize better insulation materials in retrofits
- Promote ducted, high-efficiency AC systems
- Develop income-targeted energy assistance programs

## 📁 Files
- `Code.R`: Complete analysis script
- `Code.pdf`: Annotated script output
- `Report.pdf`: Comprehensive report with visualizations and conclusions

## 🚀 Future Work
- Deploy predictive models for real-time monitoring
- Expand analysis to other high-demand months
- Integrate smart meter data for granular tracking
