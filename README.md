# 📱 Mobile Sales Analytics & Performance Dashboard

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![DAX](https://img.shields.io/badge/DAX-Data_Analysis_Expressions-0078D4?style=for-the-badge)](https://learn.microsoft.com/en-us/dax/)
[![Data Analytics](https://img.shields.io/badge/Business_Intelligence-Data_Analytics-orange?style=for-the-badge)](#)

An end-to-end Business Intelligence solution analyzing multi-brand smartphone sales across major Indian metropolitan markets from 2021 to 2024. Built with **Microsoft Power BI** and **Microsoft Excel**, this interactive dashboard delivers actionable insights into revenue performance, product popularity, geographic distribution, payment preferences, and customer satisfaction.

---

## 📌 Executive Summary & Key KPIs

Across **3,835 transactions** recorded between 2021 and 2024:

| Metric | Value | Description |
|---|---|---|
| **💰 Total Sales Revenue** | **₹76.92 Cr** (`₹769,204,988`) | Cumulative gross revenue generated |
| **📦 Total Quantity Sold** | **19,150 Units** | Overall smartphone units sold |
| **🧾 Total Transactions** | **3,835** | Number of completed customer orders |
| **📊 Average Order Value** | **₹200,575** | Average sales revenue per transaction |
| **⭐ Average Customer Rating** | **3.69 / 5.0** | Overall satisfaction score (39% 5-star ratings) |

---

## 📂 Repository Structure

```text
├── 📊 mobile sales dashboard.pbix     # Interactive Power BI Dashboard file
├── 📑 Mobile Sales Data.xlsx          # Raw dataset containing 3,835 transaction records
├── 📁 assets/                         # Visual assets and icons used in the dashboard
│   ├── mobile_logo.png
│   ├── average_icon.png
│   ├── quantity_icon.png
│   └── transactions_icon.png
├── 📄 .gitignore                      # Git ignore file for temporary & cache files
└── 📖 README.md                       # Comprehensive documentation & analytical insights
```

---

## 📊 Dashboard Visualizations & Architecture

The Power BI report (`mobile sales dashboard.pbix`) is designed with a sleek dark-blue themed layout (`#0060AA`), visual hierarchy, and cross-filtering capabilities:

### 1. 🎛️ Dynamic KPI Cards
- **Total Sales**: High-level revenue tracker with custom branding.
- **Total Quantity**: Total volume of smartphones dispatched.
- **Transactions**: Order volume monitor.
- **Average**: Real-time calculated average basket value.

### 2. 🗺️ Geographic Distribution (Bubble Map)
- Visualizes sales volume across **19 major Indian cities** (Delhi, Mumbai, Ranchi, Chennai, Bangalore, Hyderabad, Lucknow, Pune, Ahmedabad, etc.).
- Bubble size scales dynamically based on `Total Sales`.

### 3. 📈 Sales by Mobile Model (Clustered Horizontal Bar Chart)
- Ranks models by total revenue contribution.
- Highlights flagship and budget winners, led by **iPhone SE**, **OnePlus Nord**, **Galaxy Note 20**, and **Vivo Y51**.

### 4. 📉 Quantity Sold Over Time (Line Chart)
- Analyzes seasonal demand and monthly/daily trends using date hierarchy drill-downs.

### 5. 💳 Payment Method Breakdown (Donut / Pie Chart)
- Breaks down customer payment behavior across **UPI**, **Debit Card**, **Credit Card**, and **Cash**.
- Details digital payment penetration vs. traditional cash on delivery.

### 6. ⭐ Customer Satisfaction Funnel (Funnel Chart)
- Visualizes the conversion and distribution of customer feedback scores from **1-star** to **5-star**.

### 7. 📅 Sales Trend by Day of Week (Area Chart)
- Maps consumer purchasing patterns across weekdays vs. weekends (Monday through Sunday).

### 8. 🏢 Brand Performance Matrix (Summary Table)
- Comparative breakdown of all 5 major brands:
  - **Brand**
  - **Total Sales**
  - **Total Quantity**
  - **Transactions**

### 9. 🎚️ Multi-Criteria Interactive Slicers
- Slicers for rapid scenario filtering:
  - **Brand** (Apple, Samsung, OnePlus, Vivo, Xiaomi)
  - **Mobile Model**
  - **Payment Method** (UPI, Debit Card, Credit Card, Cash)
  - **Day of Week**
  - **Month Timeline Slicer**

---

## 🔍 Key Business Insights

### 🏆 1. Brand Competition: A Tight 5-Way Race
Market share is evenly balanced across the top five manufacturers, showing high competition:
- **Apple** leads in gross revenue with **₹16.16 Cr** across 783 transactions (3,932 units).
- **Samsung** is a close second with **₹16.00 Cr** across 775 transactions (3,923 units).
- **OnePlus** holds third with **₹15.37 Cr** (3,830 units).
- **Vivo** generated **₹15.01 Cr** (3,801 units).
- **Xiaomi** delivered **₹14.38 Cr** (3,664 units) with the highest average customer rating (**3.72/5.0**).

```text
Apple:   ████████████████████ 21.0% (₹16.16 Cr)
Samsung: ███████████████████  20.8% (₹16.00 Cr)
OnePlus: ██████████████████   20.0% (₹15.37 Cr)
Vivo:    ██████████████████   19.5% (₹15.01 Cr)
Xiaomi:  █████████████████    18.7% (₹14.38 Cr)
```

### 🏙️ 2. Geographic Hotspots
- **Delhi** is the dominant revenue engine, accounting for **₹20.39 Cr** (26.5% of total sales) and 1,008 transactions.
- **Mumbai** follows with **₹12.72 Cr** (16.5% of sales) across 654 transactions.
- Emerging Tier-2 markets like **Ranchi** (₹3.10 Cr), **Chennai** (₹3.08 Cr), **Rajkot** (₹2.73 Cr), and **Bangalore** (₹2.70 Cr) represent strong growth opportunities.

### 💳 3. Digital Payments Lead the Charge
- **UPI** is the single most preferred transaction channel:
  - **UPI**: ₹20.17 Cr (1,011 transactions)
  - **Debit Card**: ₹19.57 Cr (948 transactions)
  - **Credit Card**: ₹18.67 Cr (947 transactions)
  - **Cash**: ₹18.51 Cr (929 transactions)
- Over **75.9%** of all transactions were processed via non-cash / digital payment channels.

### 📅 4. Weekly Sales Cycle
- **Saturday** (₹11.44 Cr) and **Monday** (₹11.28 Cr) observe the highest purchasing velocity, indicating weekend shopping rushes and start-of-week corporate or deferred retail orders.

---

## 🗃️ Dataset Schema & Data Dictionary

The underlying dataset `Mobile Sales Data.xlsx` contains **3,835 records** across 14 attributes:

| Column Name | Data Type | Description | Example Values |
|---|---|---|---|
| `Transaction ID` | Numeric / Text | Unique identifier for each sales transaction | `1`, `2`, `3` |
| `Day` | Integer | Day of the month of purchase | `9`, `15`, `28` |
| `Month` | Integer | Month of purchase (1–12) | `10`, `11`, `12` |
| `Year` | Integer | Year of purchase (2021–2024) | `2021`, `2022`, `2023`, `2024` |
| `Day Name` | Text | Name of the day of the week | `Saturday`, `Monday`, `Sunday` |
| `Brand` | Text | Smartphone manufacturer / brand | `Apple`, `Samsung`, `OnePlus`, `Vivo`, `Xiaomi` |
| `Units Sold` | Integer | Number of units purchased in the transaction | `2`, `5`, `8` |
| `Price Per Unit` | Decimal / Float | Unit price of the smartphone model (₹) | `10174.70`, `65017.67` |
| `Customer Name` | Text | Name of the purchasing customer | `Sneha Sharma`, `Lalita Ahuja` |
| `Customer Age` | Integer | Age of customer | `18`, `32`, `45`, `51` |
| `City` | Text | City of purchase | `Delhi`, `Mumbai`, `Bangalore`, `Ranchi` |
| `Payment Method`| Text | Mode of transaction payment | `UPI`, `Credit Card`, `Debit Card`, `Cash` |
| `Customer Ratings` | Integer | Customer review rating (1 to 5) | `1`, `2`, `3`, `4`, `5` |
| `Mobile Model` | Text | Specific smartphone model variant | `iPhone 12`, `Redmi Note 10`, `Galaxy A51` |

---

## 📐 Key DAX Measures

The Power BI model incorporates core DAX measures to enable dynamic KPI calculations and cross-visual aggregation:

```dax
// 1. Total Sales Revenue
Total Sales = SUMX(Sales_Data, Sales_Data[Units Sold] * Sales_Data[Price Per Unit])

// 2. Total Units Sold
Total Quantity = SUM(Sales_Data[Units Sold])

// 3. Total Transaction Volume
Transactions = COUNTROWS(Sales_Data)

// 4. Average Sales per Transaction (Average Order Value)
Average = DIVIDE([Total Sales], [Transactions], 0)
```

---

## 🚀 Getting Started & How to Run

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Free download from Microsoft Store or official website)
- [Microsoft Excel](https://www.microsoft.com/microsoft-365/excel) (or compatible spreadsheet viewer)

### Steps to Run
1. **Clone this repository**:
   ```bash
   git clone <REPO_URL>
   cd powerbi
   ```
2. **Open the Dashboard**:
   - Double-click on `mobile sales dashboard.pbix` to launch the report in **Power BI Desktop**.
3. **Data Source Settings (If prompted)**:
   - If Power BI prompts to locate the dataset, navigate to **Home** > **Transform data** > **Data source settings**.
   - Select `Mobile Sales Data.xlsx` from your local clone path and click **Apply Changes**.
4. **Interact**:
   - Use the slicers on the left and top to filter by Brand, Model, Payment Mode, Day, and Month.

---

## 🛠️ Tech Stack & Skills Demonstrated

- **Business Intelligence**: Microsoft Power BI Desktop
- **Data Modeling & Calculations**: DAX (Data Analysis Expressions)
- **Data Preparation**: Microsoft Excel & Power Query
- **Data Visualization**: Custom KPI Cards, Geospatial Mapping, Funnel Charts, Slicers, Area Charts
- **Version Control**: Git & GitHub

---

## 👤 Author
- **Parth Garg**
- Email: `parthxgarg@gmail.com`
