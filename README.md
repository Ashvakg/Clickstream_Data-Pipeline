# ClickStream_Data-Pipeline

This project focuses on generating randomized clickstream data using Python and demonstrates how to ingest, process, and analyze this data using various AWS services including Amazon Kinesis Data Firehose, Amazon S3 acting as Datalake, AWS Glue, Amazon Athena.

# Overview

Clickstream data is a valuable source of information for understanding user behavior on websites or applications. This project simulates generating synthetic clickstream data and then showcases how to create and maintain pipeline for BI Analysts, Data Scientists.

- I am attaching the code (Main.py replace with your AWS credentials)
- Snapshots of the process
-  **Input file** which is in Json : PUT-S3-clickstreamdata-1-2024-04-23-10-02-19-92887eac-91c7-48fb-be4c-b19ce2797a69
    
  ![Data stored in S3 bucket from delivery_firehouse](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/fb0c352c-bf58-4a8d-82d8-d2c428e633eb)
  ![After crawling the json data into schema](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/fd0e4bbf-64a5-4113-a73b-d22ee9853ed1)
  ![partitions after crawling](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/bf02aee3-33b8-4d4f-aabe-7f5c77d2fb60)


- **Output Excel file** queried from Athena: Output- Structed data (Queried from Athena) in repository
  ![Queried the data using AWS Athena](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/11ca8d32-1334-4f66-8217-e3192a55b8ab)
  ![clickstream data_ready to be analysed](https://github.com/Ashvakg/ClickStream_Data-Pipeline/assets/83398283/6e235926-1eca-4c68-979c-1049c4877eb7)

# Features

- Randomized clickstream data generation using Python (code can be found in my repository).
- Ingestion of data into Amazon S3 using Amazon Kinesis Data Firehose.
- Automated schema inference and table creation with AWS Glue crawlers.
- Querying the data using Amazon Athena for insights and analytics.

# Prerequisites

- Before running this project, ensure you have the following:
- An AWS account with appropriate permissions to create and manage resources.
- AWS CLI configured with access to your AWS account.
- Python 3.x installed locally.
- Functioning knowledge of S3, Kinesis Data Delivery Firehouse, Glue, Athena to query the data

# Getting Started

1.) Clone the repository:

**git clone https://github.com/Ashvakg/ClickStream_Data-Pipeline.git**



