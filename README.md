# ClickStream_Data-Pipeline

This project focuses on generating randomized clickstream data using Python and demonstrates how to ingest, process, and analyze this data using various AWS services including Amazon Kinesis Data Firehose, Amazon S3 acting as Datalake, AWS Glue, Amazon Athena.

# Overview

Clickstream data is a valuable source of information for understanding user behavior on websites or applications. This project simulates generating synthetic clickstream data and then showcases how to create and maintain pipeline for BI Analysts, Data Scientists.

- I am attaching the code (Main.py replace with your AWS credentials)
- Snapshots of the process
- **Input file** which is in Json : PUT-S3-clickstreamdata-1-2024-04-23-10-02-19-92887eac-91c7-48fb-be4c-b19ce2797a69
- **Output Excel file** queried from Athena: Output- Structed data (Queried from Athena)

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



