# ETL_Bike_Sharing_Project
ETL Pipeline for the Bike Sharing Dataset using Python, Pandas, and NumPy.

## Dataset Description

### Data Source
The dataset used in this project is the **Bike Sharing Dataset** from the **UCI Machine Learning Repository**. It contains hourly bike rental records collected from the Capital Bikeshare system.

### Why This Dataset?
- Real-world dataset with over 17,000 records.
- Suitable for demonstrating the ETL (Extract, Transform, Load) process.
- Contains numerical, categorical, and date/time features for data transformation and analysis.

### Dataset Information
The dataset includes the following information:
- Record ID
- Date
- Month
- Year
- Hour
- Season
- Holiday
- Weekday
- Weather Condition
- Temperature
- Feels-like Temperature
- Humidity
- Wind Speed
- Casual Users
- Registered Users
- Total Rentals

### Data Type
- **Structure:** Structured data
- **Format:** CSV (Comma-Separated Values)

### Data Update Frequency
This is a historical dataset collected during **2011–2012** and is not updated regularly.

# ETL PIPELINE FLOW DIAGRAM

                 BIKE SHARING DATASET
                      (hour.csv)
                           │
                           ▼
                     Extract Data
            (Read CSV using Pandas)
                           │
                           ▼
                     Validate Data
      (Check Missing Values, Duplicates,
        Data Types, Column Information)
                           │
                           ▼
                      Clean Data
      (Remove Duplicates, Handle Missing Values)
                           │
                           ▼
                   Transform Data
       • Rename Columns
       • Convert Date to Datetime
       • Convert Year (0→2011, 1→2012)
       • Create Season_Name
       • Create Weather_Description
       • Convert Temperature to Celsius
       • Create Humidity_Level
       • Create Rental_Category
       • Sort Dataset
       • Validate Rental Values
                           │
                           ▼
                  Generate Reports
       • Cleaned Dataset
       • Top 10 Records
       • Bottom 10 Records
       • Summary Statistics
       • Monthly Rental Report
       • Weather Report
                           │
                           ▼
                        Load
      (Save Reports as CSV Files in Reports Folder)
