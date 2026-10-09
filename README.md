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

## 🔍 Insights

- **Bikes** is the top-selling category by a large margin ($148.1M net sales), followed by Clothing ($22.6M), Accessories ($12.1M), and Components ($7.5M).
- Monthly net sales stay fairly stable throughout the year (~$15.5M–$16.2M), with February as the lowest month.
- Sales are compared across **7 cities** over **3 years** (2016–2018).

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

### Database screenshots

| SalesT | Product | Location |
|---|---|---|
| ![SalesT](images/salest.png) | ![Product](images/product.png) | ![Location](images/location.png) |

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

## 🎥 Learning Resource

This project was built while following this tutorial: [Watch on YouTube](https://www.youtube.com/watch?v=eAceEDnfcPw)

## 👤 Author

**[Your Name]**
🔗 [LinkedIn]([your LinkedIn link])
