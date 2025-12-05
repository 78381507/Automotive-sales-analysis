# 📖 Data Dictionary

## Overview
This document describes the data structure, variables, and definitions used in the Automotive Sales & Service Analysis project.

---

## 📊 Dataset Information

**Source:** Kaggle - Automotive Sales Dataset  
**Time Period:** 2024 (January - December)  
**Total Records:** 58,118 transactions  
**Data Type:** Transactional sales and service data

---

## 📋 Variable Definitions

### Sales Transaction Variables

| Variable Name | Data Type | Description | Example Values |
|--------------|-----------|-------------|----------------|
| **Open Date** | Date | Date when sales transaction initiated | 2025-12-31 |
| **Month** | Text | Month of transaction | Dec, Jan, Feb, etc. |
| **Year** | Integer | Year of transaction | 2024, 2025 |
| **Days to Make** | Integer | Number of days from open to close | 1-30 |
| **Dealer ID** | Integer | Unique identifier for dealer | 1212, 1288, 1336, etc. |
| **Car ID** | Integer | Unique identifier for vehicle sold | 99110, 87110, 14110, etc. |

### Product Information

| Variable Name | Data Type | Description | Example Values |
|--------------|-----------|-------------|----------------|
| **Model** | Text | Vehicle model name | Salish, Beaufort, Labrador, Hudson, Champlain |
| **Product Line** | Text | Product category/line | Premium, Standard, Economy |

### Environmental Conditions

| Variable Name | Data Type | Description | Example Values |
|--------------|-----------|-------------|----------------|
| **Temperature (F)** | Float | Temperature at time of sale (Fahrenheit) | 33.1, 41.1, 39.9 |
| **Weather Condition** | Text | Weather status during sale | Clear, Overcast, Rain, Scattered Clouds |
| **Wind Speed (mph)** | Float | Wind speed in miles per hour | 11.5, 13.7, 19.4 |
| **Wind Direction** | Text | Cardinal direction of wind | N, S, E, W, NE, SW, etc. |
| **Humidity (%)** | Integer | Humidity percentage | 60, 68, 73 |
| **Visibility** | Float | Visibility in miles | 7, 10, 19 |
| **Wind Chill** | Float | Wind chill factor | 24.4, 29.3, 32.5 |
| **Precipitation (in)** | Float | Rainfall in inches | 0, 0.03, 0.1 |
| **Fog** | Text | Fog condition | Y, N |
| **Rain** | Text | Rain condition | Y, N |
| **Snow** | Text | Snow condition | Y, N |

### Financial Metrics

| Variable Name | Data Type | Description | Example Values |
|--------------|-----------|-------------|----------------|
| **Profit** | Currency | Profit generated per transaction | $1,181, $1,215, $1,288 |
| **Total Profit** | Currency | Aggregate profit (calculated) | $78.4M |

### Quality & Service Metrics

| Variable Name | Data Type | Description | Example Values |
|--------------|-----------|-------------|----------------|
| **Recall Status** | Boolean | Whether vehicle was recalled | Yes, No |
| **Recall Units** | Integer | Number of units affected by recall | 238K (Beaufort), 156K (Salish) |
| **System Affected** | Text | System with defect/recall | Airbag, Suspension, Engine, Seats, Tires, etc. |
| **Recall Severity** | Text | Criticality level | Critical, High, Medium, Low |

### Customer Feedback

| Variable Name | Data Type | Description | Example Values |
|--------------|-----------|-------------|----------------|
| **Sentiment** | Text | Customer sentiment classification | Positive, Neutral, Negative |
| **Sentiment Score** | Float | Numerical sentiment value | 0.58 (58% positive) |
| **Feedback Category** | Text | Type of customer feedback | Service, Quality, Sales Experience |

---

## 🔢 Calculated Metrics

### Dashboard KPIs

| Metric Name | Calculation | Description |
|------------|-------------|-------------|
| **Total Quantity Sold** | SUM(units) | Total vehicles sold across all dealers |
| **Total Profit** | SUM(profit) | Aggregate profit from all transactions |
| **Avg. Quantity Sold** | AVERAGE(units per dealer) | Average units sold per dealer |
| **Recall Rate** | (Recall units / Total units) × 100 | Percentage of units recalled |
| **Sentiment Rate** | (Positive feedback / Total feedback) × 100 | Customer satisfaction percentage |

### Performance Metrics

| Metric Name | Calculation | Description |
|------------|-------------|-------------|
| **Dealer Ranking** | RANK(profit DESC) | Dealer performance ranking by profit |
| **Model Profitability** | SUM(profit) GROUP BY model | Total profit per vehicle model |
| **Monthly Sales Volume** | COUNT(units) GROUP BY month | Units sold per month |
| **Seasonal Variance** | (Peak - Trough) / Peak × 100 | Sales volatility percentage |

---

## 📊 Data Categories

### Product Models (5 Categories)
1. **Salish** - Premium model, highest profitability
2. **Beaufort** - Standard model, quality concerns
3. **Labrador** - Mid-range model
4. **Hudson** - Economy model
5. **Champlain** - Entry-level model

### Weather Conditions (4 Primary Categories)
1. **Clear** - No precipitation, good visibility
2. **Overcast** - Cloudy conditions
3. **Scattered Clouds** - Partial cloud coverage
4. **Rain** - Active precipitation

### Sentiment Categories (3 Classifications)
1. **Positive** - Satisfied customers (58%)
2. **Neutral** - Neutral experience (28%)
3. **Negative** - Dissatisfied customers (14%)

### Recall Systems (Primary Categories)
- Airbag systems
- Suspension components
- Engine assemblies
- Seats and restraints
- Tire and wheel systems
- Visual/electrical systems
- Lights and indicators
- Powertrain components
- Other structural elements

---

## 🎯 Data Quality Notes

### Completeness
- **Complete Variables:** Dealer ID, Car ID, Model, Profit
- **Occasional Missing:** Temperature (in specific weather conditions)
- **Sparse Data:** Fog, Snow (seasonal/regional)

### Data Cleaning Applied
1. **Standardization:** Unified date formats, normalized text fields
2. **Validation:** Checked for logical consistency (e.g., profit values)
3. **Imputation:** Applied contextual filling for missing temperature data
4. **Deduplication:** Removed duplicate transaction records
5. **Outlier Treatment:** Flagged and validated extreme values

### Data Limitations
- Dataset represents single fiscal year (2024)
- Geographic information limited (no regional breakdown)
- Customer demographic data not included
- Pricing details not available (only profit shown)

---

## 📚 Data Usage Guidelines

### Recommended For:
- Sales performance analysis
- Dealer benchmarking
- Seasonal trend identification
- Quality and recall pattern analysis
- Customer sentiment tracking

### Not Suitable For:
- Individual customer profiling (no PII included)
- Precise demand forecasting (limited historical data)
- Regional market analysis (no geographic detail)
- Pricing strategy (revenue data not included)

---

## 🔄 Data Update Frequency

**Current Status:** Static dataset (2024)  
**Future Updates:** N/A (Portfolio project with fixed timeframe)  
**Refresh Strategy:** Not applicable for historical analysis

---

## 📞 Data Questions?

For questions about data definitions, calculations, or usage:
- Open a GitHub Issue
- Review PROJECT_OVERVIEW.md for detailed analysis methodology
- Contact via LinkedIn or email

---

*Last Updated: December 2024*  
*Version: 1.0*
