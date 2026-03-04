# Airbnb Booking Analysis - NYC EDA Report

## Project Overview
This project performs an Exploratory Data Analysis (EDA) on the `Airbnb_Open_Data.csv` dataset, focusing on listing characteristics, pricing trends, and geographical variations in New York City.

## Data Cleaning & Preprocessing
The following steps were taken to ensure data quality:
- **Column Normalization:** Converted all column names to lowercase and replaced spaces with underscores for easier manipulation.
- **Handling Missing Values:**
    - `last_review` was converted to datetime; missing values were filled with the minimum recorded date.
    - `reviews_per_month` missing values were filled with 0.
    - Dropped rows where essential identifiers like `name` or `host_name` were absent.
- **Price Formatting:** Handled currency strings for `price` and `service_fee`, removing symbols and converting them to float values.
- **Duplicate Removal:** Removed identical entries to maintain dataset uniqueness.

## Descriptive Statistics Summary
- **Average Listing Price:** ~$625
- **Average Service Fee:** ~$125
- **Construction Years:** Range from 2003 to 2022.
- **Review Activity:** Average of 27.5 reviews per listing, with some high-activity outliers.

## Key Insights from Visualizations

### 1. Price Distribution
The histogram reveals a wide spread of prices. While many listings cluster around lower price points, there is a visible frequency of higher-end listings, indicating a diverse market.

### 2. Room Type Popularity
A clear preference for certain room types exists, with "Entire home/apt" and "Private room" making up the bulk of the market. Shared rooms are significantly less common.

### 3. Geographical Activity
Manhattan and Brooklyn dominate in terms of listing volume, as expected for New York's primary tourist and business hubs.

### 4. Pricing by Room Type
Box plots indicate that "Entire home/apt" typically commands higher median prices and exhibits more variability compared to private or shared rooms.

### 5. Review Trends Over Time
The time-series analysis shows historical growth in Airbnb usage in NYC, reflecting increasing market maturity and traveler interest.

## Conclusion
The NYC Airbnb market is characterized by high diversity in both pricing and accommodation types. Concentration of activity is heavily biased towards Manhattan and Brooklyn, with pricing closely following the type of privacy offered by the listing.
