# Rotterdam, South Holland, The Netherlands - Data Description

**Date of Data Download:** 26 August 2024

**Source:** [Inside Airbnb](https://insideairbnb.com/get-the-data/)

## Overview

The dataset contains various CSV and GeoJSON files related to Airbnb listings in Rotterdam, South Holland, The Netherlands. These datasets include detailed information about the listings, calendars, reviews, and neighborhoods within the city. The data is useful for conducting analyses, creating visualizations, and developing insights into Airbnb usage in Rotterdam.

The version of the data is 25 June, 2024.

## File Descriptions

### 1. `listings.csv`
- **Description:** Detailed Listings data for Rotterdam.
- **Contents:** This file contains comprehensive information about Airbnb listings in Rotterdam. It includes attributes such as listing ID, host ID, neighborhood, room type, price, minimum nights, number of reviews, and many other features that describe the property and host.

### 2. `calendar.csv`
- **Description:** Detailed Calendar Data for Rotterdam.
- **Contents:** This file provides daily availability, pricing, and booking status for each listing in Rotterdam over time. It is essential for time-series analysis and understanding booking trends.

### 3. `reviews.csv.gz`
- **Description:** Detailed Review Data for Rotterdam.
- **Contents:** This file contains individual review data for listings, including review ID, date, reviewer ID, and the review text. It can be used to perform sentiment analysis or assess guest satisfaction.

### 4. `/summary/listings.csv`
- **Description:** Summary information and metrics for listings in Rotterdam (good for visualizations).
- **Contents:** This file contains a summary of the listings in Rotterdam, with aggregated metrics that are particularly suitable for visualizations and exploratory data analysis.

### 5. `/summary/reviews.csv`
- **Description:** Summary Review data and Listing ID (to facilitate time-based analytics and visualizations linked to a listing).
- **Contents:** This file provides a summary of review data, linked with listing IDs to enable time-based analytics and visualization, focusing on trends in guest reviews over time.

### 6. `neighbourhoods.csv`
- **Description:** Neighbourhood list for geo filtering. Sourced from city or open-source GIS files.
- **Contents:** This file lists all neighborhoods in Rotterdam, including relevant geographical identifiers that can be used for geospatial filtering and analysis.

### 7. `neighbourhoods.geojson`
- **Description:** GeoJSON file of neighborhoods of the city.
- **Contents:** This file provides the geographical boundaries of neighborhoods in Rotterdam, formatted as a GeoJSON file. It is suitable for creating maps and conducting spatial analysis.

## Folder Structure

- **Root Directory:** Contains the main dataset files as listed above.
- **Summary Subfolder:** The summary data files (`listings.csv` and `reviews.csv`) intended for visualizations are saved in a subfolder called `summary`.

## Usage Notes

- The detailed datasets (`listings.csv.gz`, `calendar.csv.gz`, `reviews.csv.gz`) are provided in compressed format (.gz) and need to be unzipped before use.
- Summary data files are pre-aggregated and can be used directly for visualization purposes.
- The GeoJSON file is compatible with most GIS software and can be used to visualize the spatial distribution of Airbnb listings within the city.

