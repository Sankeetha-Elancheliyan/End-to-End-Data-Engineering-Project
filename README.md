# End-to-End-Data-Engineering-Project
#COVID-19 Data Engineering Project
This repository contains the code and documentation for an end-to-end data pipeline developed to extract, transform, load, and analyze the COVID-19 dataset. The pipeline was designed using a variety of tools, and the final output was stored in Azure Synapse Analytics Database.


#Introduction
The aim of this project is to provide valuable insights on the trends in COVID-19 death rate over time. The project focuses on the ETL process and data processing, with the ultimate goal of visualizing the results in Power BI.

#Dataset Selection
The COVID-19 dataset was selected for analysis. The dataset is a centralized repository containing various sub-datasets. Therefore, only relevant subsets of the data were selected based on the insight generation mechanism.

#Insight Generation Mechanism
The data was extracted from the processed dataset and transformed into the required format. The data was then loaded from Azure Synapse Analytics database into Power BI, where various charts and graphs were created to analyze.

#Pipeline Design

![1](https://user-images.githubusercontent.com/119834420/232142894-9d23d469-91a2-45f9-bb9d-893fc4af44cf.png)

The data pipeline extracts data from the S3 bucket, transforms it using AWS Glue, and loads it into an Azure Data Lake Gen 2. Azure Synapse Analytics is used to run queries on the transformed data and connect it to Power BI for visualization.

#Technical Implementation
Python was used in Google Colab for the ETL process. Star schema was utilized to produce 4 major tables from 10 initial tables. AWS Glue was used to transform and load data into AWS Athena, and Azure Synapse Analytics to run queries on the transformed data. Further, Power BI was used for data visualization.

#Discussion and Conclusion
The project faced many challenges such as the expenditure that comes when using Redshift and the inability to connect to the cluster endpoint. Therefore, the processed data was stored in an Azure Data Lake Gen 2 instead.

In conclusion, the end-to-end solution provided insights into the impact of COVID-19 on different countries. This can be enhanced by feeding the data to machine learning algorithms to predict the spread of the pandemic, the death rate, and how effective the vaccination programs are. Also, this can be further automated using lambda functions to eradicate the need to manually do it.

Appendix


References
AWS Documentation
Azure documentation
COVID-19 Data Lake - Registry of Open Data on AWS
Azure Data Factory - Copy multiple files from AWS S3 to Azure Data Lake Storage using ADF pipeline
Azure Synapse Lakehouse with Serverless SQL and Spark Tables Tutorial
Covid_19_data_engineering_project on GitHub
