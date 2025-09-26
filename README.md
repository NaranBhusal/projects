# End-to-End Sales Analytics Pipeline in Azure

  ![image alt](https://github.com/NaranBhusal/projects/blob/b15c30070c4ba976f58879481d2833fcaccb3156/Block%20Diagram.jpg) 
  
  
  📖 Project Overview:
This project demonstrates a complete, end-to-end data engineering pipeline built using key services from the Microsoft Azure ecosystem. The goal was to ingest raw sales data, process it into a clean and structured format, store it in a high-performance data warehouse, and build an interactive dashboard for business intelligence and sales analysis. This project showcases skills in data ingestion, transformation, automation, and visualization.

---

 🏛️ Architecture
The pipeline follows a modern data warehousing architecture, moving data from a raw storage layer to a structured analytical layer, orchestrated by a central service.

The data flows through the following stages:**
1.  **Storage:** Raw, clean data (`sales_transformed.csv`) is stored in **Azure Blob Storage**.
2.  **Orchestration:** **Azure Data Factory (ADF)** automates the entire workflow. It runs a pipeline that copies the data from Blob Storage.
3.  **Data Warehousing:** The clean data is loaded into a **Azure Synapse Analytics** dedicated SQL pool. This provides a high-performance, structured data warehouse for fast and efficient querying.
4.  **Visualization:** **Power BI** connects directly to the Synapse SQL pool to create an interactive and insightful sales dashboard.

---

## 🛠️ Technologies Used
This project leverages a suite of powerful Azure services:
* **Azure Blob Storage:** For scalable and cost-effective data lake storage.
* **Azure Data Factory:** For orchestrating and automating the data pipeline.
* **Azure Synapse Analytics:** For building the central data warehouse and enabling high-speed analytics.
* **Power BI:** For creating the final business intelligence dashboard.

---

## ✨ Final Dashboard
The final result is an interactive dashboard that provides key insights into sales performance.

*Include a high-quality screenshot of your Power BI dashboard here.*
![Power BI Sales Dashboard]
![image alt](https://github.com/NaranBhusal/projects/blob/fe86309ecd4cbfa1f82c30ace01809e31f0800e9/dashboardprojectphoto.jpg)

## 🚀 How to Improve
This project serves as a strong foundation. For a production environment, I would consider the following improvements:
* **Data Transformation:** Use **Azure Databricks** to perform more complex data transformations and quality checks before loading into Synapse.
* **Security:** Use **Azure Key Vault** to manage all secrets and connection strings securely.
* **Infrastructure as Code:** Deploy all the Azure resources using **Terraform** or **ARM Templates** for better automation and environment management.
