# Airbnb Booking Analysis - NYC Exploratory Data Analysis (EDA)

## 📋 Project Overview
This project provides a comprehensive Exploratory Data Analysis (EDA) of the Airbnb dataset for New York City. The analysis focuses on listing characteristics, pricing trends, and geographical variations to uncover key insights into the NYC short-term rental market.

## 📊 Key Insights & Visualizations

### 1. Price Distribution
- **Average Listing Price:** ~$625
- **Average Service Fee:** ~$125
- **Observation:** The market shows a diverse range of pricing. While many listings are clustered in the lower price brackets, there is a significant presence of high-end luxury listings.

### 2. Room Type Popularity
- **Dominant Types:** "Entire home/apt" and "Private room" constitute the vast majority of the market.
- **Shared Rooms:** These are significantly less common, indicating a preference for privacy among NYC travelers.

### 3. Geographical Activity
- **Top Boroughs:** Manhattan and Brooklyn dominate in terms of listing volume.
- **Context:** These areas serve as the primary hubs for both tourism and business activity in New York City.

### 4. Pricing by Room Type
- **Higher Median Prices:** "Entire home/apt" generally commands higher prices compared to other types.
- **Variability:** Entire homes also show the highest variability in pricing, reflecting a wide range of accommodation quality.

### 5. Construction & Trends
- **Construction Years:** Active listings range from properties built between 2003 and 2022.
- **Market Growth:** Time-series analysis indicates a steady historical growth in Airbnb usage across the city.

## 🛠️ Data Cleaning & Preprocessing
To ensure high-quality analysis, the following steps were performed:
- **Normalization:** Column names were converted to snake_case for consistency.
- **Missing Values:**
  - `last_review` dates were filled with the minimum recorded date.
  - `reviews_per_month` missing values were set to 0.
  - Rows with missing essential fields like `name` or `host_name` were removed.
- **Data Types:** Price and service fee strings (e.g., "$193") were cleaned and converted to numerical float values.
- **Deduplication:** Identical entries were removed to maintain data integrity.

## 📈 Summary Statistics
| Metric | Value (Approx.) |
| :--- | :--- |
| Avg. Price | $625 |
| Avg. Service Fee | $125 |
| Avg. Reviews | 27.5 |
| Construction Range | 2003 - 2022 |

## 🚀 Conclusion
The NYC Airbnb market is characterized by high diversity in both pricing and accommodation types. Concentration of activity is heavily biased towards Manhattan and Brooklyn, with pricing closely following the type of privacy offered by the listing.

---
*Developed as part of the Airbnb Data Analysis Project.*
