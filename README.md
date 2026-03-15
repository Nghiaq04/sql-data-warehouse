# sql-data-warehouse
Building a modern data warehouse with SQL Server, including ETL processes, data modeling, and analytics.
📖 Project Overview

This project focuses on building a modern Data Warehouse using Microsoft SQL Server to consolidate and transform sales data from multiple source systems for analytical reporting.

The goal of this project is to demonstrate how raw operational data from different business systems can be transformed into business-ready datasets for analytics, reporting, and decision-making.

---

#🗂 Data Sources

The data used in this project comes from two business systems:

Customer Relationship Management

Enterprise Resource Planning

These systems provide operational data exported as CSV files, which are ingested into the data warehouse.

Source Files
File	Description
cust_info.csv	Customer information from CRM
prd_info.csv	Product information
sales_details.csv	Sales transaction data
CUST_AZ12.csv	Additional customer attributes from ERP
LOC_A101.csv	Customer location data
PX_CAT_G1V2.csv	Product category mapping

These files contain key business entities such as:

Customers

Products

Sales transactions

Product categories

Customer locations

---
🏗 Data Architecture

The project follows the Medallion Architecture with three layers:

🥉 Bronze Layer – Raw Data

The Bronze layer stores raw data ingested directly from the source CSV files.

Characteristics:

Data is loaded as-is

No transformations are applied

Tables represent the raw structure of the source systems

Data is loaded using bulk ingestion processes

Purpose:

Preserve original data

Enable data traceability

Provide a backup of source data

---
🥈 Silver Layer – Cleaned & Standardized Data

The Silver layer performs data cleaning and transformation.

Typical transformations include:

Removing duplicate records

Handling missing values

Standardizing categorical values (e.g., gender, marital status)

Data type conversion

Creating derived columns

Data normalization

At this stage, the data becomes consistent and analysis-ready.

---
🥇 Gold Layer – Business-Ready Data

The Gold layer contains analytical data models optimized for reporting and analytics.

Key characteristics:

Business logic applied

Data integration across CRM and ERP sources

Aggregations and metrics

Analytical data structures

Data models may include:

Star schema

Fact tables

Dimension tables

This layer is designed for:

Business Intelligence reporting

Analytical queries

Data exploration

---
📊 Analytics Use Cases

The data warehouse enables analysis across several business domains:

Customer Analysis

Customer demographics

Customer segmentation

Customer purchase behavior

Product Performance

Best-selling products

Product category performance

Revenue by product line

Sales Analysis

Sales trends over time

Order and shipment performance

Revenue and quantity analysis

⚙️ Technologies Used

SQL development using Microsoft SQL Server

Data ingestion from CSV files

ETL processes implemented using SQL

Data modeling techniques used in Data Warehouse systems

---
🎯 Learning Objectives

This project demonstrates practical skills in:

SQL development

Data ingestion and ETL pipelines

Data cleaning and transformation

Data warehouse architecture

Data modeling for analytics

It is designed as a hands-on learning project for students and professionals interested in:

Data Engineering

Data Analytics

Data Architecture

Business Intelligence
