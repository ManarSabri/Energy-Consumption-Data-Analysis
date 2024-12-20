# Energy Consumption Data Analysis  

A comprehensive project analyzing energy consumption data collected from network sites. This project provides actionable insights into energy usage patterns, identifies key drivers of consumption, and proposes strategies for optimization and cost reduction.

---

## Table of Contents  

- [About the Project](#about-the-project)  
- [Objectives](#objectives)  
- [Dataset Description](#dataset-description)  
- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [Setup Instructions](#setup-instructions)  
- [Usage](#usage)  
- [Analysis Details](#analysis-details)  
- [Contributing](#contributing)  
- [License](#license)  

---

## About the Project  

This project focuses on analyzing energy consumption data collected from network sites. The primary objective is to monitor and track energy usage to uncover patterns and derive actionable insights.  
By leveraging statistical analysis and visualization techniques, the project validates assumptions and proposes strategies to optimize energy consumption, supporting better energy management and cost reduction decisions.  

---

## Objectives  

- Analyze the dataset to extract meaningful insights about energy consumption across different network sites.  
- Validate the following assumptions using statistical tests:  
  - Does the region significantly affect energy consumption?  
  - Is there a relationship between the time of day and energy consumption?  
- Identify low-consumption cells and estimate potential energy and cost savings in case of shutdowns.  

---

## Dataset Description  

The dataset contains detailed information about energy consumption from network sites, covering various metrics and time intervals. Below are the dataset columns and their descriptions:  

| **Column**                 | **Description**                                                               |  
|----------------------------|-----------------------------------------------------------------------------|  
| `cell_id`                  | Unique identifier for each cell.                                            |  
| `DateTime`                 | Timestamp for the half-hour interval.                                       |  
| `KWH/hh (per half hour)`   | Energy consumption (in kWh) per half-hour interval.                         |  
| `site_id`                  | Unique identifier for each site.                                            |  
| `region`                   | Region associated with the site.                                            |  
| `Demand`                   | Categorical representation of demand.                                       |  
| `DemandPrice`              | Price associated with demand.                                               |  
| `Cost_per_half_hour`       | Cost (in £) per half-hour interval.                                         |  
| `Region_Avg_KWH`           | Average energy consumption (in kWh) for the region.                        |  
| `Region_Avg_Cost`          | Average cost (in £) for the region.                                         |  
| `Site_Total_KWH`           | Total energy consumption (in kWh) for the site.                            |  
| `Site_Total_Cost`          | Total cost (in £) for the site.                                             |  
| `Hour`                     | Hour of the day (0-23).                                                     |  
| `Day_of_Week`              | Day of the week (0 for Monday, 6 for Sunday).                               |  
| `Month`                    | Month of the year (1 for January, 12 for December).                         |  

---

## Features  

- **Data Cleaning and Preprocessing:**  
  - Standardization of time intervals and handling of missing data.  
  - Removal of duplicates and invalid rows.  

- **Feature Engineering:**  
  - Mapping demand levels to pricing tiers.  
  - Region-specific and time-based metrics for analysis.  

- **Outlier Detection and Handling:**  
  - Identification and processing of abnormal energy usage patterns.  

- **Statistical Testing:**  
  - Hypothesis testing for consumption differences across regions and times.  
  - Correlation analysis between demand price and consumption costs.  

- **Optimization Strategies:**  
  - Threshold determination for low-consumption cells to estimate energy and cost savings.  

---

## Technologies Used  

- **Python**  
- **Pandas** for data manipulation.  
- **NumPy** for numerical computations.  
- **Matplotlib** and **Seaborn** for visualizations.  
- **Scipy** for statistical hypothesis testing.  
- **Jupyter Notebook** for interactive analysis.  

---

## Setup Instructions  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/energy-analysis.git
