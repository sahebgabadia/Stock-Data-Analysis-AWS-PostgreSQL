# Real-Time Stock Market Data Analysis Using AWS and PostgreSQL


**Setup 1: EC2-RDS (PostgreSQL) for Stock Data Analysis**

**Components:**
1. CSV File: Contains stock data with 9 columns (Index, Date, High, Open, Low, Close, Adj_Close, Volume, Close_USD).

2. Python Script: Simulates real-time stock data analysis.
   
3. AWS EC2 (Elastic Compute Cloud): Hosts the Python script and manages the connection to RDS.
   
4. AWS RDS (Relational Database Service): PostgreSQL database to store and manage stock data.

**Workflow:**
1. Python Script Execution: The Python script runs on an EC2 instance. This script is responsible for loading the stock data into RDS, simulating a real-time environment.
   
2. Querying Data: Uses SQL queries via PostgreSQL for data manipulation and retrieval.
   
3. Data Processing: The PostgreSQL database on RDS is used to perform real-time analysis of stock data (such as calculating moving averages, identifying trends, etc.).
 
4. Data Output: The output can be in the form of reports or visualizations.




**Setup 2: EC2-S3-Athena for Stock Data Analysis**

**Components**
1. CSV File: Same stock data file as in Setup 1.
   
2. Python Script: Simulates real-time stock data analysis.
   
3. AWS EC2: Hosts the Python script.
   
4. AWS S3: Stores stock data.
   
5. AWS Athena: Serverless query service to perform SQL queries on data stored in S3.

**Workflow**
1. Python Script Execution: The Python script runs on an EC2 instance. This script is responsible for loading the stock data into S3, simulating a real-time environment.
   
2. Querying Data: Uses SQL queries via AWS Athena for data manipulation and retrieval.
   
3. Data Processing: Athena queries the stock data stored in S3 to perform analysis based on the query results (e.g., trend analysis, volatility computation).
   
4. Data Output: The output can be in the form of reports or visualizations.
