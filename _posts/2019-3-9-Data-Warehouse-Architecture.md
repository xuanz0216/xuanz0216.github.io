---
layout: post
title: Data warehouse architecture
date: 2019-03-09
category: Data Warehouse
---
A **data-warehouse** collects data from multiple sources and organises under a unified schema. There are two approaches for constructing data-warehouse. **Top-down approach** and **Bottom-up approach**. Below will explain **Top-down approach**.

**1. Top-down approach**
*  external sources
* staging area : since the data, extracted from the external sources does not follow a particular format, so there is a need to validate this data to load into data warehouse. 
* Data warehouse: After cleaning of data, it is stored in the data warehouse as central repository. It actually stores the meta data and the actual data gets stored in the data marts. Note that data warehouse stores the data in its purest form in this top-down approach.
* Data Marts: Data Mart is also a part of storage component. It stores the information of a particular function of an organization which is handled by single authority.
* Data mining 
This approach is defined by **Inmon** as - data warehouse as a central repository for the complete organisation and data marts are created from it after the complete data warehouse has been created.

**2. Three-tier data warehouse architecture**
Generally, a data warehouse adopts a three-tier architecture.
* 