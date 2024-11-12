# 9.1 Requirements Gathering Conversation

The text describes a mock stakeholder interview between a data engineer (Joe) and a data scientist (Colleen) discussing data engineering requirements for a marketing analytics project.

## Key Challenges:
* Colleen currently receives daily data dumps from the sales platform
* She spends about 80% of her time cleaning and processing data
* The data is often 2 days old, which doesn't meet marketing team's need for real-time analytics
* Processing scripts frequently crash due to data format changes or anomalies

## Current Marketing Analytics Needs:
1. Dashboards showing:
   * Product sales by category and region
   * 30-day totals and timeline plots
   * Ability to drill down into specific regions and products
2. Product Recommendation System:
   * Currently shows generally popular products
   * Goal is to develop a personalized recommendation system using content filtering
   * Want to recommend products to customers while browsing or making purchases

## Proposed Solutions:
* Develop a more direct and timely data ingestion process
* Automate data transformation and serving
* Create a system that can provide near real-time data for marketing insights

## Next Steps:
* Joe will follow up with the marketing team to understand their precise data timeliness requirements
* Aim to create a more efficient data pipeline that reduces manual processing and enables faster insights

The conversation demonstrates the importance of requirements gathering in data engineering projects and how collaboration between data engineers and data scientists can improve data workflows.
