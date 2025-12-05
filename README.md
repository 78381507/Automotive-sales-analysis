# 🚗 Automotive Sales & Service Analytics

A comprehensive data analysis project examining automotive sales performance, dealer efficiency, product line profitability, and customer sentiment across a major automotive sales network.

![Dashboard Preview](assets/dashboard_preview.png)

## 📊 Project Overview

This project analyzes automotive sales and service data to uncover actionable insights about product performance, dealer effectiveness, seasonal trends, and customer satisfaction. The analysis combines sales metrics, recall data, and sentiment analysis to provide a 360-degree view of business performance.

**Key Performance Indicators:**
- **Total Units Sold:** 58,118 vehicles
- **Total Profit:** $78.4M
- **Average Units Sold per Dealer:** 19.37 vehicles
- **Customer Sentiment:** 58% positive ratings

## 🎯 Key Insights

### 1. Product Line Performance
- **Top Performer:** Salish model generates highest profitability at $34M
- **Underperformer:** Beaufort model shows concerning performance with significant losses
- **Recommendation:** Investigate Beaufort's cost structure and consider discontinuation or redesign

### 2. Dealer Analysis
- **Best Dealer:** Dealer #1288 achieves peak performance with $9.6M in profit
- **Consistency:** Top 5 dealers maintain $8-9M profit range
- **Worst Performer:** Dealer #1222 generates only $6.2M (35% below best dealer)

### 3. Seasonal Trends
- **Peak Season:** May shows highest sales at 5.8K units
- **Sales Drop:** August experiences 35% decline vs peak (3.6K units)
- **Strategic Insight:** Align inventory and marketing budget with seasonal patterns

### 4. Quality & Customer Satisfaction
- **Recall Risk:** Beaufort accounts for 24% of all recalls (238K units) - critical concern
- **Sentiment Analysis:** 58% positive customer feedback indicates room for improvement
- **Root Cause:** Airbag, suspension, and engine issues are primary recall drivers

## 🛠️ Technologies & Tools

- **Data Cleaning:** Google Sheets
- **Data Visualization:** Looker Studio
- **Data Source:** Kaggle automotive dataset
- **Analysis Methods:** Statistical analysis, trend identification, comparative analysis

## 📁 Project Structure

```
automotive-sales-analysis/
│
├── README.md                          # Project documentation
├── data/
│   ├── raw/                          # Original Kaggle dataset
│   └── cleaned/                      # Cleaned data in Google Sheets
│
├── dashboard/
│   └── Automotive_Sales_Dashboard.pdf # Looker Studio dashboard export
│
└── assets/
    └── dashboard_preview.png         # Dashboard screenshots
```

## 📈 Dashboard Components

The interactive dashboard includes:

1. **Executive Summary Cards**
   - Total quantity sold
   - Overall profit
   - Average units per dealer

2. **Dealer Performance Analysis**
   - Profit distribution across all dealers
   - Best/worst performer identification
   - Performance benchmarking

3. **Product Line Breakdown**
   - Profit by model (Salish, Beaufort, Labrador, Hudson, Champlain)
   - Sales volume comparison

4. **Quality Metrics**
   - Recall distribution by product line
   - Root cause analysis by system (airbag, suspension, engine, etc.)
   - Critical recall threshold monitoring

5. **Customer Voice**
   - Sentiment breakdown (Positive, Neutral, Negative)
   - Customer satisfaction trends

6. **Temporal Analysis**
   - Monthly sales evolution
   - Seasonal pattern identification
   - Year-over-year comparison

## 🔍 Methodology

### Data Cleaning Process
1. **Data Import:** Sourced automotive sales dataset from Kaggle
2. **Quality Check:** Identified missing values, duplicates, and outliers
3. **Standardization:** Normalized date formats, dealer IDs, and product names
4. **Enrichment:** Added calculated fields (profit margins, dealer rankings)
5. **Validation:** Cross-checked totals and ensured data consistency

### Analysis Approach
- Comparative analysis across dealers and product lines
- Time-series analysis for seasonal trends
- Root cause analysis for recalls and quality issues
- Sentiment analysis of customer feedback

## 💡 Business Recommendations

1. **Immediate Actions:**
   - Launch urgent investigation into Beaufort model quality issues
   - Implement dealer training program based on #1288's best practices
   - Increase marketing spend in March-April to maximize May peak

2. **Strategic Initiatives:**
   - Develop recall prevention protocol focused on airbag and suspension systems
   - Create August sales promotion to counter seasonal decline
   - Expand successful Salish model production capacity

3. **Performance Optimization:**
   - Establish dealer performance scorecards
   - Implement early warning system for quality issues
   - Enhance customer satisfaction programs to reach 70%+ positive sentiment

## 🎓 Skills Demonstrated

- Data cleaning and preparation
- Business intelligence dashboard creation
- Statistical analysis and trend identification
- Data storytelling and visualization
- Stakeholder-focused insights generation
- Quality assurance and validation

## 📫 Contact

**François**  
Aspiring Data Analyst | Data Engineering Enthusiast

- LinkedIn: [Your LinkedIn Profile]
- GitHub: [Your GitHub Profile]
- Email: [Your Email]

---

## 📄 License

This project is available for educational and portfolio purposes.

## 🙏 Acknowledgments

- Dataset source: Kaggle
- Visualization platform: Looker Studio
- Data processing: Google Sheets
