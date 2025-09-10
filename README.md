# Urban Mobility Patterns Analysis

**Project – Big Data**  
*Bachelor in Digital Technologies, AI & Decision Support Systems*

For this project, two complementary datasets related to urban mobility in Great Britain were used. The first, “local_authority_traffic”, contains detailed traffic information by region, including road length and vehicle counts. The second, “UK_Accident”, includes detailed records of individual traffic accidents, covering location, severity, weather, and road conditions.

Both datasets were imported into MongoDB ("mobilidade" database with "acidentes" and "contagem" collections) and processed with PySpark using the mongo-spark-connector. Data was converted to Parquet for efficiency, columns were renamed for consistency, and records were filtered to 2005–2014. Irrelevant columns and duplicates were removed, datasets were joined on authority_id and year, and missing values were handled with appropriate defaults. Additional features, such as period_of_day, were created to enrich analysis.

This preprocessing ensured clean, consistent, and relevant data, ready for exploratory and advanced analysis of urban mobility patterns and traffic safety.

## Features
- Batch and advanced data processing with PySpark  
- Data storage and querying with MongoDB  
- Exploratory and advanced analysis of urban mobility trends  
- Visualizations with Matplotlib and Seaborn  
- Automated reports generation  

## Tech Stack
- MongoDB  
- PySpark  
- Python (Matplotlib, Seaborn, Pandas)  

## How to Run
1. Start MongoDB and import datasets.  
2. Install Python dependencies.  
3. Run scripts in `/scripts` for data processing and analysis.  
4. Explore notebooks in `/notebooks` for visualizations and insights.

