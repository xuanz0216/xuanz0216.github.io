---
layout: post
title: Data Lake
date: 2019-03-09
category: Data Warehouse
---

A data lake is a storage repository that can store large amount of structured, semi-structured, and unstructured data. It offers high data quality to increase analytics performance and native integration.

Unlike a hierarchal data warehouse where data is stored in files and folder. Data lake has a flat architecture. Every data element in a data lake is given a unique identifier and tagged with a set of metadata information.

**1. Why data lake**
1. Data lake offers business agility
2. Can keep unrefined view of data

**2. Data lake architecture**
* **Ingestion tier**
* **Insights tier**
* **HDFS** is a cost-effective solution for both structured and unstructured data. It is the landing zone for all data
* **Distillation tier** takes data from the storage tier and converts it to structured data for easier analysis
* **Process tier** run analytical algorithms and users queries
* **Unified operation tier** governs system management and monitoring. It includes auditing and proficiency management, data management and workflow management.
**3. Key concepts in data lake**
* Data ingestion
* Data storage
* Data governance
* Data security
* **Data quality**
* **Data lineage**