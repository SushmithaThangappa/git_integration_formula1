**Project Description**

This project implements an end-to-end data engineering solution for analyzing and reporting on Formula 1 motor racing data using Azure Databricks and Azure Data Lake. The solution demonstrates core principles of cloud data engineering, focusing on secure data access, automation, and visualization.

**Key Features**

**1. Secure and Simplified Data Access**

Mounted Azure Data Lake Storage using a service principal to securely access and manage data.

Integrated Azure Key Vault for securely storing credentials, ensuring sensitive information like passwords and storage account keys remain hidden.

Eliminated the need for long URLs by leveraging secrets from Key Vault for streamlined code.

**2. Automated Pipeline Execution**

Designed and implemented a tumbling window trigger to automate the execution of Databricks notebooks.

Automated the ingestion of race data from the raw layer to the processed layer in the Azure Data Lake.

Built robust mechanisms to handle missing files gracefully, ensuring pipeline reliability and data integrity.

**3. Transformation and Reporting**

Triggered transformation and reporting notebooks upon successful data ingestion, implementing a multi-stage pipeline workflow.

Created transformation logic to calculate race results, driver standings, and constructor standings.

**4. Continuous Integration and Deployment (CI/CD)**

Integrated GitHub with Azure Data Factory (ADF) to enable version control and automate the CI/CD process.

Streamlined collaboration and deployment workflows for pipeline updates and releases.

**5. Interactive Dashboards**

Developed interactive dashboards in Databricks to visualize key insights such as:

**Race results

Driver standings

Constructor standings**

Exported dashboards as HTML files for easy sharing and offline viewing.

6. Exclusion of Delta Lake

Focused on leveraging core Azure Databricks and Azure Data Lake capabilities without implementing Delta Lake, ensuring a simpler architecture.

**Technologies Used**

Azure Services

Azure Databricks

Azure Data Lake Storage Gen2

Azure Key Vault

Azure Data Factory

Version Control and CI/CD

GitHub

Data Processing

Spark (PySpark)

Visualization

Databricks Dashboards

HTML Exports


**Future Enhancements**

Implement Delta Lake to enhance reliability and enable advanced features such as ACID transactions and time travel.

Add support for real-time data processing using Spark Streaming.

Expand visualizations with more interactive features and external tools like Power BI.
