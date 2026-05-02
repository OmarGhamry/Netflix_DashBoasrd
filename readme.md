# Netflix Data Dashboard & ETL Project
## Project Overview

This project involves a comprehensive end-to-end data analysis of the Netflix titles dataset. The goal was to transform raw, semi-structured CSV data into a functional Star Schema to support a high-performance interactive dashboard. The final product provides deep insights into Netflix's content distribution, growth trends over time, and key contributors across the globe.

![Netflix Dashboard](/images/image.png)



### Data Source
[Source File](/Dataset/netflix_titles.csv)

### Description 
The dataset contains over 8,800 records of movies and TV shows available on Netflix as of 2021, including details on cast, directors, ratings, and release years.

### Data Architecture
To move away from a flat-file structure and optimize for analytical queries, the data was modeled into a relational schema:

Schema Design
Fact Table (show_info): Acts as the central hub containing primary attributes such as show_id, title, type, and release_year.

Dimension Tables: Dedicated tables were created to handle multi-valued attributes (many-to-one relationships), including:

show_director

show_cast

show_genre

show_country

Dashboard Features
The final dashboard provides a visual narrative of Netflix’s library:

Key Performance Indicators (KPIs): High-level metrics showing the total show count (~9K), recent additions, and content density.

Content Composition: A donut chart displaying the ratio between Movies and TV Shows.

Geographic Analysis: A bar chart identifying the United States and India as the leading content producers.

Star Power Tracking: Analysis of the most frequent cast members, highlighting actors like Anupam Kher.

Temporal Trends: A line graph tracking "Shows Count Over Time," illustrating the massive surge in content production between 2015 and 2019.

Advanced Filtering: Interactive slicers for Country, Rating, and time periods (Year, Quarter, Month).

Tools & Technologies
Data Modeling: Star Schema / Normalization

Analysis: Power Query for data cleaning and string splitting

Visualization: Power BI / Data Visualization Suite

How to Use
Clone the repository.

Ensure the dataset netflix_titles.csv is in the root directory.

Run the ETL scripts to normalize the data into the defined schema.

Open the Dashboard file to explore the interactive visuals.