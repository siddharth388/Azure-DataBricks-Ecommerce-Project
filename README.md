# Azure-DataBricks-Ecommerce-Project!

Technology Stack - 
1. Microsoft Azure (Azure Data Lake Gen2, Azure Data Factory)
2. Azure Databricks
3. Apache Spark
4. Delta Lake

Microsoft Azure - 
In Microsoft Azure I have used services like Azure Data Lake Gen2 and Azure Data Factory for this project. Azure Data Lake Gen2 allows you to store data in a directory and sub-directory structure. Azure Data Factory is used here to ingest the data from Github repo and store it in the Azure data lake and then apply basic transformation like changing the file format from .csv to .parquet format.

Azure Databricks - 
Azure Databricks is a platfrom where you can run PySpark code for furthur transformation of your dataset.

Apache Spark - 
Apache Spark is used to apply transformation on the data. I have used the Medallion Architecture (Bronze - Silver - Gold) of Databricks to process the data. Bronze layer is just a layer where we load and store the data. In Silver layer we apply transformation as per Business logics and the Gold layer is where I have aggregated the table. I have used the concept of One Big Table (OBT) in the Gold Layer.

Delta Lake - 
Delta Lake is an open source storage layer which brings together the benefits of both Data Lake and Data Warehouse. At the end of the project I have converted the One Big Table to Delta format Table and done some analysis using SQL in Databricks.


![Architecture Diagram](https://github.com/user-attachments/assets/aa60b843-0bf8-4316-b825-8c69a0869108)
