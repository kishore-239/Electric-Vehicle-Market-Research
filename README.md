[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://python.org)
[![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow)](https://powerbi.microsoft.com)
[![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-green)](https://pandas.pydata.org)
[![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-Web_Scraping-orange)](https://www.crummy.com/software/BeautifulSoup/)

# ⚡ EV Market Analysis: From Web Scraping to Interactive Dashboard

**A comprehensive Electric Vehicle market analysis project combining Python-based data collection with Power BI dashboard visualization.**

If you find this project useful, please consider starring ⭐ the repository or connecting with me on LinkedIn.

---

## 📌 Project Overview

A comprehensive **Electric Vehicle (EV) market analysis** project combining **Python-based data collection/EDA** with an **interactive Power BI dashboard**. The project extracts real-world EV data, analyzes performance metrics, and visualizes insights through a professional business intelligence dashboard.

## 🎯 Project Components

### **1. Data Collection & Analysis (Python)**
**Tools:** BeautifulSoup, Requests, Pandas, NumPy, Matplotlib, Seaborn  
**Files:** `webscraping_EV.ipynb`, `EDA_EV_Data.ipynb`

**Key Analysis:**
- Scraped **973 EV models** from automotive sources
- Analyzed relationships between **price, range, battery capacity, and acceleration**
- Identified strong correlation between battery capacity and range (**r = 0.90**)
- Discovered **brand-level performance patterns** across 74 manufacturers

### **2. Interactive Dashboard (Power BI)**
**Tools:** Power BI Desktop, Power Query, DAX  
**Files:** `EV_Dashboard.pbix`

**Dashboard Features:**
- **Single-page analytical overview** of global EV market
- **Interactive filters:** Brand, Year, Price Segment (Budget/Mid-Range/Premium)
- **KPIs:** Total Models (973), Average Price (€48.19K), Average Range (376 km)
- **Visualizations:** Price vs Range scatter plot, Brand comparison, Market trends

## 📊 Key Insights

### **Quantitative Findings**
| Metric | Value |
|--------|-------|
| **Total Models Analyzed** | 973 |
| **Average Price** | €48,187 |
| **Average Real-World Range** | 376 km |
| **Average Battery Capacity** | 71.2 kWh |
| **Brands Covered** | 74 |

### **Analytical Insights**
- **Strong correlation** between battery capacity and range (**r = 0.90**)
- **Weak correlation** between price and range (**r = 0.10**) - brand/technology matter more
- **Tesla** and **Audi** lead in performance and efficiency
- **EV range** has steadily increased over the past decade

## 🔍 Key Visualizations

### **1. Interactive Dashboard**
![EV Dashboard Preview](https://github.com/kishore-239/Electric-Vehicle-Market-Research/raw/main/images/dashboard_screenshot.png)

**Power BI Dashboard Features:**
- Interactive price vs range scatter plot
- Brand-level performance comparison
- Market segmentation analysis
- Historical range improvement trends
- KPI tracking: 973 models, €48.19K avg price, 376 km avg range

### **2. Market Overview - Brand Distribution**
![Brand Distribution Pie Chart](https://github.com/kishore-239/Electric-Vehicle-Market-Research/raw/main/images/step5_brand_distribution_PieChart.png)

**Key Insights:**
- **Market Leaders:** Mercedes-Benz (8%), Volkswagen (7%), and Tesla (6.5%) lead the EV market — together contributing over **20% of total models**.
- **Top 10 brands** capture ~50% of the market, showing moderate **concentration** among established automakers.
- **European dominance:** Strong presence of German and French brands (Mercedes, VW, Audi, BMW, Peugeot, Renault, Citroën).
- **Fragmented tail:** "Others" category forms ~36% of the market, reflecting **many small players** and ongoing diversification.

**Summary:** The EV market is competitive, with established European leaders at the top and a long tail of emerging brands — a hallmark of an expanding and innovative industry.

### **3. Correlation Analysis - Performance Relationships**
![Correlation Heatmap](https://github.com/kishore-239/Electric-Vehicle-Market-Research/raw/main/images/step6_correlation_heatmap.png)

**Distribution Insights:**
- **Price (€):** Right-skewed distribution, indicating most EVs are mid-priced, with fewer high-end luxury models above €80,000.
- **Real-World Range (km):** Roughly normal distribution centered around **375 km**, showing most EVs fall between **300–450 km** range.
- **Battery Capacity (kWh):** Concentrated around **70–80 kWh**, with a few large-capacity models (100 kWh +).
- **Energy Efficiency (Wh/km):** Mostly between **170–210 Wh/km** — lower values indicate higher efficiency.

**Correlation Insights (Pearson Method):**
- **Battery Capacity ↔ Real-World Range:** Strong **positive correlation (~ 0.9)** — larger batteries lead to longer range.
- **Battery Capacity ↔ Fast Charging Speed:** Moderate **positive correlation (~ 0.75)** — larger packs often support faster charging.
- **Range ↔ Acceleration:** **Negative correlation (~ –0.7)** — faster cars (lower 0–100 s) tend to have shorter ranges due to higher power demand.
- **Price ↔ Range/Battery:** Weak positive correlation — higher-priced EVs *tend* to have better specs, but not always directly proportional.

**Summary:** This univariate analysis reveals balanced numeric distributions for most technical attributes with clear physical relationships between **battery, range, and performance**.

### **4. Bivariate Analysis - Key Relationships**
![Scatter Relationships](https://github.com/kishore-239/Electric-Vehicle-Market-Research/raw/main/images/step7_scatter_relationships.png)

**Observations from Correlation Analysis:**
- **Battery Capacity ↔ Real-World Range (r = 0.90):** The strongest relationship — larger batteries directly lead to longer driving range.
- **Battery Capacity ↔ Fast Charging Speed (r = 0.75):** Bigger batteries tend to support faster charging systems.
- **Range ↔ Fast Charging Speed (r = 0.72):** Long-range EVs often come with higher charging speeds.
- **Acceleration ↔ Range / Battery Capacity (r ≈ −0.7):** Faster cars (lower acceleration time) are typically less efficient and have smaller range.
- **Price ↔ Range (r = 0.10):** Only a weak link — price doesn't scale directly with range, possibly due to luxury brand pricing strategies.

**Summary:** The EV market shows clear engineering patterns — larger batteries drive performance and charging speed, while speed performance comes at the cost of range and efficiency.

### **5. Brand Performance Comparison**
![Brand Boxplots](https://github.com/kishore-239/Electric-Vehicle-Market-Research/raw/main/images/step8_boxplots_brands.png)

**Insights from Brand-wise Averages:**
| Brand | Avg. Price (€) | Avg. Range (km) | Avg. Battery (kWh) | Avg. Efficiency (Wh/km) | Avg. Acceleration (sec) |
|:------|---------------:|----------------:|-------------------:|------------------------:|-------------------------:|
| Audi | 57,078 | 442 | 85.4 | 195.6 | 5.7 |
| BMW | 49,157 | 419 | 77.1 | 182.1 | 5.5 |
| Ford | 62,150 | 381 | 76.4 | 202.8 | 6.4 |
| Mercedes-Benz | 50,140 | 439 | 86.6 | 203.7 | 6.9 |
| Peugeot | 46,389 | 272 | 54.7 | 206.8 | 11.1 |
| Tesla | 46,092 | 437 | 78.7 | 181.3 | 4.6 |
| Volkswagen | 54,432 | 380 | 70.6 | 191.1 | 7.8 |
| Volvo | 58,803 | 394 | 78.7 | 199.8 | 5.9 |

**Performance & Efficiency Trends:**
- **Tesla, Mercedes-Benz and Audi** lead the market in **range** (~ 440 km) while maintaining **excellent efficiency** (~180–196 Wh/km).
- **Peugeot** is the most **budget- and efficiency-oriented**, but offers the **lowest range** (≈270 km) and **slowest acceleration** (~11 sec).
- **Luxury brands** (Audi, Mercedes-Benz, Volvo) maintain **larger battery packs** (~80–87 kWh) for long-range capability.
- **Ford** shows **higher prices** (€62 K on avg) despite moderate range (381 km), suggesting strong brand pricing or high-end trims.

### **6. Multivariate Analysis - Battery vs Range by Brand**
![Battery vs Range Top Brands](https://github.com/kishore-239/Electric-Vehicle-Market-Research/raw/main/images/step10_battery_vs_range_top_brands.png)

**Brand-Level Patterns:**
- **Tesla** and **Mercedes-Benz** lead in **range and capacity**, emphasizing performance.
- **Volkswagen** and **BMW** balance range, cost, and efficiency.
- **Peugeot** and smaller brands focus on affordability, with modest specs.
- Most **discontinued EVs** had **lower range and smaller batteries**, hinting at outdated tech.

**Summary:**
- **Battery size** is the dominant driver of EV range and performance.
- **Performance–Range trade-off** exists: faster EVs travel less per charge.
- **Price** has limited correlation with technical specs — brand value and features drive pricing.
- The EV market clearly segments into **budget, mid-range, and premium tiers**.

**In short:** *Battery capacity is the engine of range and performance — while price follows brand and design more than engineering specs.*

*📊 All 26 EDA visualizations are available in the [`eda/`](https://github.com/kishore-239/Electric-Vehicle-Market-Research/tree/main/images) folder of this repository.*

## 🛠️ Technical Skills Demonstrated

### **Data Engineering**
- Web scraping with BeautifulSoup and Requests
- Data cleaning and transformation using Pandas
- Handling missing values and outliers

### **Data Analysis & Statistics**
- Exploratory Data Analysis (EDA)
- Correlation analysis and hypothesis testing
- Trend identification and pattern recognition

### **Data Visualization**
- Static visualizations with Matplotlib/Seaborn (Python)
- Interactive dashboard creation with Power BI
- DAX measures for calculated metrics
- Professional dashboard design and layout

### **Business Intelligence**
- KPI definition and tracking
- Market segmentation analysis
- Competitive benchmarking
- Data-driven storytelling

## 📁 Project Structure
```text
Electric-Vehicle-Market-Research/
│
├── data_collection/
│ ├── webscraping_EV.ipynb
│ └── raw_data.csv
│
├── data_analysis/
│ ├── EDA_EV_Data.ipynb
│ ├── cleaned_data.csv
│ └── eda/ (26 visualization files)
│
├── dashboard/
│ ├── EV_Dashboard.pbix
│ └── dashboard_screenshot.png
│
├── images/
│ ├── dashboard_screenshot.png
│ ├── correlation_heatmap.png
│ ├── price_distribution.png
│ └── battery_vs_range.png
│
└── README.md
```


## 🚀 How to Use This Project

### **For Data Scientists/Analysts:**
1. Run `webscraping_EV.ipynb` to collect latest EV data
2. Execute `EDA_EV_Data.ipynb` for exploratory analysis
3. Review all 26 visualizations in the `eda/` folder

### **For Business Users:**
1. Open `EV_Dashboard.pbix` in Power BI Desktop
2. Use slicers to filter by Brand, Year, or Price Segment
3. Explore relationships through interactive visualizations
4. Click "Reset Filters" to return to default view

## 💼 Business Impact
- **Manufacturers:** Evaluate competitive positioning and pricing strategies
- **Consumers:** Make informed decisions based on performance-price trade-offs
- **Analysts:** Identify market trends and innovation patterns
- **Investors:** Assess market maturity and growth opportunities

## 🏷️ Keywords
`EV Market Analysis` · `Web Scraping` · `Exploratory Data Analysis` · `Power BI Dashboard` · 
`Data Visualization` · `Electric Vehicles` · `Business Intelligence` · `Python` · 
`Pandas` · `BeautifulSoup` · `Seaborn` · `DAX` · `Automotive Analytics` · 
`Battery Technology` · `Market Segmentation` · `Competitive Analysis`

## 📫 Contact
**Email:** [kishorekrishna623@gmail.com](mailto:kishorekrishna623@gmail.com)  


