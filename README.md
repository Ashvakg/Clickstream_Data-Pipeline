### **Objective**
This project aims to develop an efficient and scalable solution for handling clickstream data, enabling stakeholders to gain valuable insights into user behavior and interactions.
Kinesis Firehose is chosen in this project for its seamless integration with other AWS services, scalability and durability for handling batch of streamed data, which often generated continuosly and requires real-time processing for analysis and insights.

### **Input file** in Json : PUT-S3-clickstreamdata-1-2024-04-23-10-02-19-92887eac-91c7-48fb-be4c-b19ce2797a69

### **Approach**
  - **Inception**: Inspired by the importance of clickstream data in understanding user behavior, the project commenced with the objective of building a robust data pipeline for its processing and analysis.
  - **Data Ingestion**: Clickstream data is ingested into the pipeline using Kinesis Firehose, which streams the data directly to S3, creating a data lake for storage and further processing.
    ![Data stored in S3 bucket from delivery_firehouse](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/fb0c352c-bf58-4a8d-82d8-d2c428e633eb)
    
  - **Data Processing**: AWS Glue is employed for data processing tasks such as data cleaning, transformation, and schema inference. Glue's serverless and scalable nature ensures efficient processing of large volumes of clickstream data.
    ![After crawling the json data into schema](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/fd0e4bbf-64a5-4113-a73b-d22ee9853ed1)
    ![partitions after crawling](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/bf02aee3-33b8-4d4f-aabe-7f5c77d2fb60)
    
  - **Data Analysis**: Clickstream data stored in the S3 data lake is queried using AWS Athena, enabling ad-hoc SQL queries for analysis. Athena's interactive query performance allows for rapid exploration and visualization of insights derived from the clickstream data.

### **Output** queried from Athena:
Output structed data (queried from Athena) present in repository
  ![Queried the data using AWS Athena](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/11ca8d32-1334-4f66-8217-e3192a55b8ab)
  ![clickstream data_ready to be analysed](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/6e235926-1eca-4c68-979c-1049c4877eb7)

### **Features**
- Randomized clickstream data generation using Python (code can be found in my repository).
- Ingestion of data into Amazon S3 using Amazon Kinesis Data Firehose.
- Automated schema inference and table creation with AWS Glue crawlers.
- Querying the data using Amazon Athena for insights and analytics.
