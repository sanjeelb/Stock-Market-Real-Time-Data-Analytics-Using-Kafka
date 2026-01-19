# Stock-Market-Real-Time-Data-Analytics-Using-Kafka

## Overview

This project demonstrates an end-to-end data engineering pipeline for **real-time stock market data** using Apache Kafka and various AWS services. The pipeline ingests stock market data, processes it, and stores it in a structured format for analytics.

The main objective is to build a **robust, scalable, and real-time data pipeline** capable of handling high-frequency stock market data for analytics and business intelligence.

---

## Goal / Purpose

The goal of this project is to provide a practical example of a **real-time data engineering workflow** for financial data, enabling:

- Real-time ingestion and processing of stock market data  
- Seamless integration with AWS services (S3, Glue, Athena)  
- Analytics-ready storage for dashboards and reporting  
- Hands-on experience with Apache Kafka for streaming pipelines  

---

## Technologies Used

- **Programming Language**: Python  
- **Data Streaming**: Apache Kafka  
- **Cloud Services**:
  - AWS S3 (Simple Storage Service)  
  - AWS Glue Crawler & Catalog  
  - AWS Athena  
  - AWS EC2  
- **Data Format**: CSV  
- **Data Processing**: AWS Glue, Athena  

---

## Architecture

The pipeline architecture consists of:

1. **Data Ingestion**: Fetch stock market data using `yfinance` Python library  
2. **Data Streaming**: Stream data in real-time with Apache Kafka  
3. **Data Storage**: Store streamed data in AWS S3 buckets  
4. **Data Processing**:  
   - AWS Glue Crawler to infer schema and create Glue Catalog  
   - AWS Athena to query structured data stored in S3  
5. **Data Consumption**: Analytics, dashboards, or reporting  

![Architecture Diagram](./Architecture.jpg)

---

## Dataset

The dataset contains historical stock market data in CSV format:

- `indexProcessed.csv`: Historical stock prices and trading data for selected indices  
