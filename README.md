# Uber Data Analytics | Modern Data Engineering GCP Project

![00](https://github.com/themihirmathur/Uber-Data-Analytics/assets/92594107/5014bc9d-4477-4a5e-ab94-4f320f86f44c)

## Introduction

The goal of this project is to perform comprehensive data analytics on Uber trip data using a modern data engineering stack on Google Cloud Platform (GCP). This project leverages various GCP services and tools to extract, transform, and load (ETL) the data, and ultimately visualize the insights gained from the analysis. The key components of this project include GCP Storage, Python, Compute Instance, Mage Data Pipeline Tool, BigQuery, and Looker Studio.

## Architecture

![Screenshot 2024-07-05 at 8 30 36 PM](https://github.com/themihirmathur/Uber-Data-Analytics/assets/92594107/e1888bea-6382-4678-b22c-864bee15e0e3)

The architecture for this project follows a robust and scalable design:

1. **Data Ingestion**:
   - **GCP Storage**: Raw data is stored in Google Cloud Storage, providing a durable and highly available repository for data.
   
2. **Data Processing**:
   - **Compute Instance**: Python scripts running on GCP Compute Instances to clean and preprocess the data. Compute Instances offer flexible, scalable virtual machine resources for various workloads.
   - **Mage Data Pipeline Tool**: Used to automate the ETL processes and manage data workflows. Mage simplifies building, running, and monitoring data pipelines.
   
3. **Data Warehousing**:
   - **BigQuery**: Processed data is stored in BigQuery for efficient querying and analysis. BigQuery is a fully-managed, serverless data warehouse that enables super-fast SQL queries using the processing power of Google's infrastructure.
   
4. **Data Visualization**:
   - **Looker Studio**: Dashboards and reports are created in Looker Studio to visualize the insights from the data analysis. Looker Studio allows creating interactive, sharable reports and dashboards with Google Analytics data.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Technology Used

- **Programming Language**: Python
  - Python is used for data processing and analysis due to its simplicity and the vast array of libraries available for data manipulation, such as Pandas, NumPy, and Scikit-learn.
- **Google Cloud Platform**:
  - **Google Storage**: A scalable, secure, and highly available object storage service.
  - **Compute Instance**: Virtual machine instances that provide the compute capacity for running data processing scripts.
  - **BigQuery**: A managed data warehouse for storing and querying large datasets efficiently.
  - **Looker Studio**: A business intelligence tool for creating data visualizations and dashboards.
- **Modern Data Pipeline Tool**: Mage ([Mage](https://www.mage.ai/))
  - Mage is a modern data pipeline tool that allows for easy ETL workflows and automation of data processing tasks.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Dataset Used

The dataset used for this project is the TLC Trip Record Data, which includes yellow and green taxi trip records. These records capture various fields such as:

- **Pick-up and drop-off dates/times**: The start and end times of each trip.
- **Pick-up and drop-off locations**: Latitude and longitude coordinates of trip origins and destinations.
- **Trip distances**: The distance traveled during each trip.
- **Itemized fares**: Breakdown of fare components including base fare, taxes, and surcharges.
- **Rate types**: Fare rate categories such as standard, flat rate, or negotiated.
- **Payment types**: Methods of payment used for the trip, such as credit card, cash, or no charge.
- **Driver-reported passenger counts**: Number of passengers reported by the driver for each trip.

**Dataset Source**: [Uber Data CSV](https://github.com/themihirmathur/Uber-Data-Analytics/tree/main/data)

**More Information**:
- **Website**: [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- **Data Dictionary**: [TLC Data Dictionary](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf)

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Data Model

![00](https://github.com/themihirmathur/Uber-Data-Analytics/assets/92594107/b805b069-8294-4329-bcf9-21b115d93bfa)

The data model for this project is designed to support efficient querying and analysis. It includes the following tables:

- **Trip Data**: Contains detailed records of each trip including timestamps, locations, distances, fares, and passenger counts.
- **Location Data**: Contains metadata about the pick-up and drop-off locations.
- **Fare Data**: Contains itemized fare details for each trip.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## ETL Process

1. **Extraction**: Raw trip data is extracted from the source and loaded into GCP Storage. This ensures the data is durably stored and easily accessible for further processing.
2. **Transformation**: Data cleaning and preprocessing are performed using Python scripts running on GCP Compute Instances. The Mage Data Pipeline Tool is used to orchestrate and manage these processes. Transformations include data normalization, filtering out erroneous entries, and enriching the data with additional context.
3. **Loading**: The cleaned and transformed data is loaded into BigQuery for storage and querying. BigQuery's powerful SQL engine allows for fast and efficient analysis of the data.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Data Analysis

The analysis focuses on uncovering insights such as:

- **Peak hours for trips**: Identifying the busiest times of the day for taxi rides.
- **Most popular pick-up and drop-off locations**: Determining the locations with the highest number of trips.
- **Average trip distances and fares**: Calculating the typical distance and cost of a trip.
- **Payment method distribution**: Analyzing the proportion of different payment methods used.
- **Passenger count trends**: Examining the distribution of passenger counts across trips.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Visualization

The results of the data analysis are visualized using Looker Studio, providing interactive dashboards and reports that stakeholders can use to gain actionable insights. These visualizations help in understanding patterns and trends in the data, making it easier to make data-driven decisions.

![Screenshot 2024-07-05 at 8 38 51 PM](https://github.com/themihirmathur/Uber-Data-Analytics/assets/92594107/def82c0c-9e26-420e-87b9-682d280562ac)
![Screenshot 2024-07-05 at 8 37 37 PM](https://github.com/themihirmathur/Uber-Data-Analytics/assets/92594107/117a5e15-34c8-4c20-aa0f-4db35dbd0ac5)

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>

## Conclusion

This project demonstrates the use of modern data engineering practices and tools to perform data analytics on Uber trip data. By leveraging GCP services and the Mage Data Pipeline Tool, the project achieves a scalable and efficient ETL process, enabling comprehensive analysis and visualization of the data.

---

Feel free to contact me for any questions or further information.

**Contacts**  
Email: [themihirmathur@gmail.com](mailto:themihirmathur@gmail.com)  
LinkedIn: [linkedin.com/in/mihirmathur](https://www.linkedin.com/in/mihirmathur)  
GitHub: [github.com/themihirmathur](https://github.com/themihirmathur)

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="1920" 
</p>
