# Kathiyawadi Restaurant Market Pricing — Ahmedabad

## Project Overview

This project analyzes the vegetarian Kathiyawadi restaurant market
in Ahmedabad to support pricing decisions for a new restaurant
planned near Sindhu Bhavan, Ahmedabad.

The analysis focuses on competitor restaurants, restaurant ratings,
dish-level menu prices, food categories and market price benchmarks.

---

## Business Objective

The objective is to understand the current market pricing of
vegetarian Kathiyawadi food and identify appropriate pricing
benchmarks for a new restaurant in Ahmedabad.

---

## Key Business Questions

- What is the average market price of each dish?
- What is the median price?
- What are the minimum and maximum observed prices?
- Which restaurants have higher menu prices?
- Do highly rated restaurants charge higher prices?
- Which food categories have higher prices?
- What is the observed price range for common Kathiyawadi dishes?
- How do competitor restaurants compare in terms of pricing?

---

## Dataset

The project uses three related tables:

### 1. Restaurant

Contains restaurant-level information.

Columns:

- Restaurant_ID
- Restaurant_Name
- City
- Area
- Restaurant_Type
- Cuisine
- Restaurant_Rating
- Review_Count
- Price_Range
- Source_URL

### 2. Product

Contains dish-level information.

Columns:

- Product_ID
- Dish_Name
- Food_Category
- Sub_Category
- Cuisine_Type
- Cooking_Medium

### 3. Fact_Menu_Price

Contains restaurant menu pricing information.

Columns:

- Menu_Price_ID
- Restaurant_ID
- Product_ID
- Price
- Portion_Size
- Serving_Unit
- Dish_rating
- Menu_Type
- Source_URL
- Price_Date

---

## Power BI Dashboard

The dashboard contains two main pages.

### Page 1 — Kathiyawadi Restaurant Market Pricing — Ahmedabad

Includes:

- Market Average Price
- Median Price
- Minimum Price
- Maximum Price
- Number of Restaurants
- Number of Dishes
- Average Price by Dish
- Average Price by Food Category
- Market Price Range by Dish
- Restaurant Rating vs Average Menu Price

<img width="1335" height="732" alt="image" src="https://github.com/user-attachments/assets/caccda79-e795-49a0-a90a-fbb63a7ed9cd" />

### Page 2 — Competitor Pricing Analysis

Includes:

- Restaurant Price Comparison
- Average Price by Restaurant
- Restaurant filter
- Area filter
- Dish filter
- Food Category filter
  
<img width="1328" height="742" alt="image" src="https://github.com/user-attachments/assets/53fc055d-e0c0-4f54-9377-a58c771754bf" />

---

## Power BI Data Model

The data model consists of:

Restaurant
        |
        | Restaurant_ID
        |
Fact_Menu_Price
        |
        | Product_ID
        |
Product

This model allows the dashboard to dynamically analyze
restaurant and dish-level pricing.

---

## Data Sources

Menu and restaurant information was collected from publicly
available online sources.

Source URLs are provided in the dataset and/or
`sources/source_urls.csv`.

The project does not estimate or fabricate menu prices.
Where information was unavailable, the corresponding field
was left blank.

---

## Important Data Limitations

- Some restaurants do not provide complete information for
  ratings, reviews, portion sizes, or cooking medium.
- Cooking medium is only recorded where explicitly available.
- Prices represent observed listed menu prices and should be
  interpreted as market benchmarks rather than guaranteed prices.
- Some dishes have fewer restaurant observations than others.

---

## Tools Used

- Power BI
- Power Query
- DAX
- Excel 
- Web Research

---

## Project Files

| File | Description |
|---|---|
| `README.md` | Project documentation and methodology |
| `Restaurant.xlsx` | Restaurant-level data |
| `Product.xlsx` | Dish/product-level data |
| `Fact_Menu_Price.xlsx` | Menu pricing data |
| `powerbi/Kathiyawadi_Restaurant_Market_Pricing.pbix` | Power BI dashboard |
| `dashboard/page1_market_overview.png` | Dashboard Page 1 preview |
| `dashboard/page2_competitor_analysis.png` | Dashboard Page 2 preview |

###### Kathiyawadi_Market_Data.xlsx contain Restaurant.xlsx and Fact_Menu_Price.xlsx
---


