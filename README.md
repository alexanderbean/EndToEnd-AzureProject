# EndToEnd-AzureProject

This is my first data engineering project and my first non-academic project.

My goal in this project was to learn more about the development stages in a data engineering pipeline, and to gain hands-on practice with the Azure cloud platform and its many tools.

In this project, I used:
- Azure Gen2 Data Lake Storage
- Azure Data Factory
- Azure Databricks
- Azure SQL Database
- SQL Server Management Studio
- Power BI Desktop

These are the major steps I took in creating this end-to-end project:
- I created the resource group to house the applicable deployed services listed above.
- I added three BLOB storage containers in Azure Gen2 Data Lake Storage for staging data, raw data, and transformed data.
- I then imported data from local .csv files into the staging data container.
- In Data Factory, I developed a pipeline to copy the staging data into the raw data container, to separate what would be the "Bronze" and "Silver" layers.
- Transformed the raw data in Databricks using pySpark and some imported SQL functions. I then saved this new data into the transformed data container.
- In SSMS, I assigned the table schemas and developed a pipeline to load the transformed data into Azure SQL Database.
- Back in Data Factory, I developed a pipeline to load the transformed data from BLOB storage into Azure SQL Database.
- I then pulled the data stored in Azure SQL Database into Power BI Desktop.


I established a Git repo connection to Data Factory after all the pipelines were completed.
