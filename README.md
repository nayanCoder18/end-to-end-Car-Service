# 🚗 End-to-End Car Services Analysis  

## 📌 Project Overview  
This project is an **end-to-end data analysis pipeline** focused on the automotive services domain (car sales, insurance, and service history). The goal was to integrate multiple datasets, clean and transform them, perform in-depth SQL-based analysis, and finally build interactive visualizations in Power BI.  

## 📊 Data Sources  
The dataset was originally downloaded from **Kaggle** and cleaned using **Excel** to handle missing, null, and blank values before importing into SQL.  

### Tables Used  
1. **car_data** → Car specifications and pricing details  
   - *(Car_ID, Brand, Model, Year, Fuel_Type, Transmission, Color, Owner_Type, Mileage_kmpl, Price_Lakh)*  

2. **insurance_data** → Insurance details and policy status  
   - *(Car_ID, Provider, Policy_Number, Expiry_Date, Status)*  

3. **owner_data** → Owner information and purchase year  
   - *(Car_ID, Owner_Name, Contact, City, Purchase_Year)*  

4. **sales_data** → Sales transaction details  
   - *(Car_ID, Sale_Price_Lakh, Sale_Date, Buyer_Name)*  

5. **service_history** → Car servicing history and costs  
   - *(Car_ID, Service_Type, Service_Date, Service_Cost, Service_Center)*  

## 🛠️ Tools & Technologies  
- **Excel** → Data Cleaning  
- **SQL Server** → Database & Analysis  
- **Power BI** → Visualization & Reporting  

## 📝 Project Steps  

### Step 1: Data Collection  
- Downloaded datasets from Kaggle.  
- Datasets include car specifications, sales, insurance, owners, and service history.  

### Step 2: Data Cleaning (Excel)  
- Removed duplicates, null, and blank values.  
- Standardized date formats and categorical fields.  
- Ensured data consistency across all tables.  

### Step 3: Database Integration & Data Analysis (SQL Server)  

**SQL Analysis Examples:**  

| Analysis | Columns Used |
|----------|--------------|
| Total Cars | `Car_ID` |
| Total Sales Value | `Sale_Price_Lakh` |
| Total Brands | `Brand` |
| Total Models | `Model` |
| Total Car Sales per Year | `Sale_Date`, `Sale_Price_Lakh` |
| Count of Cars by Fuel Type | `Fuel_Type` |
| Total Automatic vs Manual Cars | `Transmission` |
| Total Car Sales per Model | `Model`, `Sale_Price_Lakh` |
| Top 10 Cities with Highest Car Sales | `City`, `Car_ID` |
| Total Cars by Insurance Status | `Status` |
| Average Car Price | `Price_Lakh` |
| Relationship between Car Mileage & Price | `Mileage_kmpl`, `Price_Lakh` |
| Total Service Cost per Year | `Service_Date`, `Service_Cost` |
| Total Service Cost per Service Type | `Service_Type`, `Service_Cost` |
| Total Cars by Owner Type | `Owner_Type` |
| Top 10 Buyers by Number of Purchases | `Buyer_Name`, `Car_ID` |
| Trend of Car Sales by Fuel Type Over Years | `Sale_Date`, `Fuel_Type`, `Sale_Price_Lakh` |

### Step 4: Data Visualization (Power BI)  

| Visualization | Chart Type | Columns Used | Suggested Colors |
|---------------|------------|--------------|-----------------|
| Summary KPIs | Card | Total Cars, Total Sales, Total Brands, Total Models | Default KPI colors (blue, green, orange) |
| Sales by Year | Column Chart | `Sale_Date` (Year), `Sale_Price_Lakh` | Blue gradient |
| Cars by Fuel Type | Horizontal Bar | `Fuel_Type`, `Car_ID` | Different color per fuel type (Petrol - #FF7F50, Diesel - #1E90FF, Electric - #32CD32) |
| Manual vs Automatic | Pie Chart | `Transmission` | Manual - #FF8C00, Automatic - #4682B4 |
| Car Sales by Model | Donut Chart | `Model`, `Sale_Price_Lakh` | Gradient by model count |
| Top 10 Cities by Ownership | Bar Chart | `City`, `Car_ID` | City-wise gradient |
| Insurance Status | Pie Chart | `Status` | Active - #32CD32, Expired - #FF4500 |
| Average Price by Brand | Column Chart | `Brand`, `Price_Lakh` | Brand-wise color palette |
| Mileage vs Price Correlation | Scatter Plot | `Mileage_kmpl`, `Price_Lakh` | Points - #1E90FF |
| Service Cost Trend by Year | Line Chart | `Service_Date` (Year), `Service_Cost` | Line - #FF6347 |
| Service Cost by Service Type | Bar Chart | `Service_Type`, `Service_Cost` | Different color per service type |
| Owner Type Distribution | Pie Chart | `Owner_Type` | 1st Owner - #32CD32, 2nd Owner - #FFD700, Others - #FF69B4 |
| Top Buyers | Table | `Buyer_Name`, `Sale_Price_Lakh` | Default table styling |
| Fuel Type Trend over Years | Stacked Column | `Sale_Date` (Year), `Fuel_Type`, `Sale_Price_Lakh` | Fuel-type specific colors |

---

## 📈 Key Insights & Use Cases  
- Identified **top-selling brands, models, and cities**  
- Evaluated **fuel type and transmission preferences**  
- Tracked **insurance coverage** and **service costs**  
- Correlated **mileage with price trends**  

## 🚀 Outcome  
This project demonstrates a **complete analytics workflow** from raw data to actionable business insights, showcasing skills in **data cleaning, SQL queries, database design, and Power BI dashboard creation**.
