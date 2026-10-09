# 📊 Sales Dashboard – Power BI

An interactive sales dashboard built with **Power BI**, analyzing **3M+ sales records** stored in a **Microsoft Access** database across products, cities, and time.

## 🖼️ Dashboard Preview

![Dashboard](images/dashboard.png)

## 🎯 Key Metrics

| Metric | Value |
|---|---|
| Gross Sales | $217.6M |
| Net Sales | $190.4M |
| Discount Value | $27.2M |
| Total Quantity | 6M |

## 📈 Visuals Included

- Net Sales by Year and City (ribbon chart)
- Net Sales by Month (area chart)
- Gross Sales by Month (donut chart)
- Net Sales by Category (funnel chart)
- Net Sales by Year
- KPI cards: Gross Sales, Net Sales, Discount Value, Quantity

## 🗄️ Data Model

The data comes from a Microsoft Access database (`SalesDB`) with 3 tables:

| Table | Description |
|---|---|
| **SalesT** | Sales transactions (~3.1M rows): `ProductID`, `CityCode`, `Date`, `Quantity`, `Discount` |
| **Product** | Products: `ProductID`, `ProductName`, `Category`, `Price` |
| **Location** | Cities: `City`, `CityCode` (7 cities) |

Relationships:
- `SalesT.ProductID` → `Product.ProductID`
- `SalesT.CityCode` → `Location.CityCode`

## 📥 Data

The full database (`SalesDB.accdb`, 3M+ records) is too large for GitHub.

👉 [Download the database from Google Drive](https://drive.google.com/file/d/1Wnfce9xaebiQy3kHzfuboHhF7b5sz2hD/view?usp=sharing)

> The `.pbix` file already contains the data, so you can open the dashboard without downloading the database.

## 🛠️ Tools Used

- Power BI Desktop
- Microsoft Access
- DAX

## 🚀 How to Use

1. Download `sales.pbix` from this repository.
2. Open it with **Power BI Desktop**.
3. Explore the visuals and use the filters.

## 👤 Author

**[Hanan Radad]**
