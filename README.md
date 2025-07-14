# 🏠 Dubai Housing Market Dashboard

This project provides a data-driven analysis of Dubai's residential real estate market using a dataset of 50,000 property listings. The goal is to help buyers, investors, and real estate professionals better understand property trends through an interactive **Power BI dashboard**.

## 📊 Project Overview

- **Dataset**: 50,000 residential listings in Dubai
- **Tool Used**: Power BI
- **Deliverables**: Interactive dashboard, data cleaning pipeline, and insights report

## 📁 Dataset Details

| Column Name     | Description                        |
|----------------|------------------------------------|
| SquareFeet      | Size of the property               |
| Bedrooms        | Number of bedrooms                 |
| Bathrooms       | Number of bathrooms                |
| Neighborhood    | Urban / Suburb / Rural             |
| YearBuilt       | Year the property was built        |
| Price           | Listed price in AED                |

### 🔧 Additional Calculated Fields

- `PricePerSqft = Price / SquareFeet`
- `PropertyAge = 2025 - YearBuilt`
- `ListingCategory`: Budget / Mid-Range / High-End *(based on price quantiles)*

## 🧹 Data Cleaning

- Removed negative and duplicate records
- Fixed column data types
- Filtered prices to realistic range: **25,000–500,000 AED**
- Ensured no missing values

## 📈 Dashboard Features

- **KPI Cards**: Total Listings, Avg Price, Highest Price, Avg Price/Sqft, Avg Property Size
- **Charts**:
  - Bar chart: Avg Price by Neighborhood
  - Stacked Column: Listings by Bedrooms & Category
  - Treemap: Listings by Area & Category
  - Scatter Plot: SquareFeet vs Price
  - Histogram: Property Age Distribution
- **Slicers**: Bedrooms, Bathrooms, Neighborhood, Listing Category, Price

## 🔍 Key Insights

1. **More Realistic Prices** after cleaning (Avg ~225,000 AED)
2. **Urban Homes Are Pricier**, while rural/suburban are more affordable
3. **Most Listings Are Family-Sized** (2–4 bedrooms)
4. **High-End Urban Homes Dominate Market Value**
5. **Size and Price Are Strongly Correlated**
6. **Dubai Has a Modern Housing Stock** (Most homes <50 years)


