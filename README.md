# Seattle Airbnb Data Analysis

## Overview
This project explores Airbnb listings in Seattle using [Kaggle](https://www.kaggle.com/datasets/alexanderfreberg/airbnb-listings-2016-dataset) data from 2016. The dataset consists of three sheets: Listings, Reviews, and Calendar. Using Tableau, I performed several joins and visualized key insights such as price trends, location-based pricing, and the impact of property size on rental prices. The goal is to determine optimal strategies for hosting Airbnb properties in Seattle, focusing on price and availability.

## Project Details

### 1. Dataset
- **Listings Sheet**: Contains details about the properties, including location, type of property, number of beds/baths, and prices (daily, weekly, monthly).
- **Reviews Sheet**: Includes review ID, listing ID, and review comments.
- **Calendar Sheet**: Tracks the availability of listings (occupied or vacant) for each date, using `listing_id` for identification.

### 2. Data Preparation in Tableau
- Imported the `listings.csv` file into Tableau.
- Performed joins on the `listing_id` field between the Listings, Calendar, and Reviews tables.
- Due to the dataset’s size (23 million rows), applied filters to focus on data from 2016 and excluded the Reviews table to reduce the dataset to around 10 million rows.

### 3. Key Visualizations
#### **Price by Zipcode (Sheet 1)**
- Visualized the average price for Airbnb listings by Seattle zip codes.
- **Purpose**: Identify the most expensive areas to guide real estate investment for Airbnb properties.
- **Visualization Type**: Bar chart labeled as "Price by Zipcode."

#### **Price per Zipcode Map (Sheet 2)**
- Created a map using zip codes, with colors representing average prices in each area.
- **Purpose**: Display the geographic distribution of rental prices across Seattle.
- **Visualization Type**: Map, labeled "Price per Zipcode."

#### **Revenue per Year (Sheet 3)**
- Analyzed weekly revenue trends across 2016, filtered by calendar dates.
- **Purpose**: Determine the best time to list properties for maximum revenue.
- **Visualization Type**: Line chart, labeled "Revenue per Year."

#### **Average Price per Bedroom (Sheet 4)**
- Explored how the number of bedrooms impacts the average price of listings.
- **Purpose**: Assess which property sizes are most profitable for Airbnb rentals.
- **Visualization Type**: Bar chart, labeled "Average Price per Bedroom."

#### **Distinct Count of Bedroom Listings (Sheet 5)**
- Displayed the number of listings based on the number of bedrooms, with null and zero-bedroom listings filtered out.
- **Purpose**: Understand the availability of different property sizes.
- **Visualization Type**: Bar chart, labeled "Distinct Count of Bedroom Listings."

### 4. Final Dashboard
- Combined all visualizations into a comprehensive dashboard named **Airbnb Full Project**.
- **Purpose**: Provide a full view of the pricing and availability trends for Airbnb listings in Seattle.

## Tools Used
- **Tableau Public**: Used for data preparation, joining, and visualizing.
- **Excel (CSV)**: Data source containing the 2016 Seattle Airbnb listings, reviews, and calendar information.

## How to Use
1. **Open Tableau Workbook**: Access the workbook via Tableau Public to explore the visualizations and interact with the dashboard.
2. **Explore Visualizations**: Use filters to adjust the data, and drill down into specific zip codes, property types, or price ranges.
3. **Understand the Insights**: Use the dashboard to identify the most profitable areas, optimal pricing strategies, and the best times to list properties.

## File Structure
- `README.md`: This project description.
- `data/`: Contains the CSV files with Airbnb listings, reviews, and calendar data.
- `tableau/`: Tableau workbook with all visualizations and the final dashboard.

## Key Insights
- Zip code-based price trends can help potential Airbnb hosts decide where to buy properties.
- One-bedroom properties in Seattle are performing well based on average price per day.
- Revenue trends suggest there are certain times in the year that are more profitable for listing properties on Airbnb.

## Future Enhancements
- Include data from 2021 for a broader analysis of recent trends.
- Integrate additional metrics like occupancy rates and guest reviews for a deeper analysis.
