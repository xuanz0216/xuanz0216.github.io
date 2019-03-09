---
layout: post
title: Data Modeling
date: 2019-03-09
category: Data Warehouse
---
In this post. We first understand the goals of data warehouse and business intelligence, then explore dimensional modeling core concepts and establish fundamental vocabulary.

**1. What is dimensional model**
A dimensional model is a data structure technique optimized for data warehouse tools. A dimensional model is designed to read, summarize, analyze numeric information in the data warehouse.
In contrast, relational data model is designed to add, update, remove records in a real-time online transaction system.

**2. Elements of dimensional data model**
* Fact are the metrics/measurements from your business process
* Dimension give who (customer), what(product), where(location) of a fact
* Attributes location(state, country, zipcode)
* Fact table is a primary table in a dimensional model. A fact table contains fact, foreign key to dimension table

**3. Steps of dimensional modelling**
* select the business process
* declare the level of detail
> if a table contains sales data for every day, then it should be daily granularity. If a table contains total sales data for each month, then it has monthly granularity.
* identify dimension (what, where, who)
* identify fact
* build the schema
> star schema 
    The star schema architecture is easy to design. The central of the star consists of the fact table and the points of the start is domension tables.
    The fact table in the star chema which is third normal form.
    The dimensional table are de-normalized
> snowflake schema
    The snowflake schema is an extension of the star schema, ecah dimension are normalized and connected to more dimension tables
