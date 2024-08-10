# Sales Data Engineering Project

This project showcases an end-to-end data engineering pipeline developed for processing and analyzing sales data. The solution leverages various Azure services to ingest, transform, store, and visualize sales data, ensuring efficient data processing and governance.

## Project Overview

The project involves the following key components:

1. **Ingestion and Storage**
   - **Data Source:** On-premise SQL Server database.
   - **Ingestion Tool:** Azure Data Factory.
   - **Storage:** Azure Data Lake.

   Data from the SQL Server is ingested using Azure Data Factory and securely stored in Azure Data Lake for further processing.

2. **Transformation and Loading**
   - **Transformation Tool:** Azure Databricks.
   - **Loading Destination:** Azure Synapse Analytics.

   The raw data stored in Azure Data Lake is transformed using Azure Databricks to achieve the cleanest form, which is then loaded into Azure Synapse Analytics for further analysis.

3. **Visualization and Governance**
   - **Visualization Tool:** Power BI.
   - **Governance Tools:** Azure Active Directory (AAD) and Azure Key Vault.

   An interactive dashboard was built in Power BI, integrated with Azure Synapse Analytics, to visualize the sales data. Azure Active Directory and Azure Key Vault were implemented to monitor and ensure governance across the pipeline.


### Detailed Workflow

1. **Data Ingestion**
   - Data Factory pipelines were created to extract data from the on-premise SQL Server.
   - Data was securely transferred and stored in Azure Data Lake.

2. **Data Transformation**
   - Azure Databricks notebooks were used to clean and process the raw data.
   - Transformation scripts ensured data was in the optimal format for analysis.

3. **Data Loading**
   - The clean data was loaded into Azure Synapse Analytics for further use in reporting and analytics.

4. **Data Visualization**
   - Power BI was connected to Azure Synapse Analytics to create real-time, interactive dashboards.
   - Dashboards provided insights into sales trends, performance metrics, and other key business indicators.

5. **Monitoring and Governance**
   - Azure Active Directory (AAD) was used to manage access control and user authentication.
   - Azure Key Vault was implemented for secure management of secrets and keys across the project.

## Prerequisites

To replicate this project, ensure you have the following:

- Azure Subscription
- SQL Server database with sales data
- Access to Azure Data Factory, Azure Data Lake, Azure Databricks, Azure Synapse Analytics, Power BI, Azure Active Directory, and Azure Key Vault
- Basic understanding of Azure services and data engineering concepts

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/sales-data-engineering.git
   ```

2. **Configure Azure Services:**
   - Set up Azure Data Factory to connect to your on-premise SQL Server.
   - Create Azure Data Lake storage for raw data ingestion.
   - Set up Azure Databricks and Azure Synapse Analytics for data transformation and storage.

3. **Run the Pipelines:**
   - Trigger Azure Data Factory pipelines to ingest data.
   - Execute Databricks notebooks for data transformation.
   - Load the transformed data into Azure Synapse Analytics.

4. **Visualize the Data:**
   - Connect Power BI to Azure Synapse Analytics.
   - Create and publish dashboards for data visualization.

## Security and Governance

- **Azure Active Directory (AAD):** Used for managing access control and ensuring secure authentication.
- **Azure Key Vault:** Implemented for managing secrets, keys, and other sensitive information securely.

## Conclusion

This project demonstrates a comprehensive data engineering pipeline for sales data, utilizing Azure's robust ecosystem to manage, transform, and visualize data effectively. The solution ensures data integrity, security, and governance while providing actionable insights through interactive dashboards.

## License

This project is licensed under the [MIT License](LICENSE).


