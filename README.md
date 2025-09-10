# MICROSOFT FABRIC BOOTCAMP – LEARNING JOURNEY

This repository documents hands-on exercises completed during the Microsoft Fabric Bootcamp. It covers key concepts such as Lakehouse, Warehouse, Data Pipelines, and practical experience with Dataflow Gen2 and Power Query transformations within Microsoft Fabric.

---

## 📅 Week 1

### Class 1: Introduction to Microsoft Fabric
- What is Microsoft Fabric?
- Key Features of Microsoft Fabric
- Overview of OneLakehouse architecture
- Microsoft Fabric components and ecosystem
- Use cases and business value

---

### Class 2: Workspace and Lakehouse Concepts
1. Free Mirroring Storage </br>
- Understanding the benefits of mirrored data storage for reliability.

2. Who Should Use Microsoft Fabric</br>
- Identifying target users and organizations for Fabric adoption.

3. OneLake Overview</br>
- Introduction to Microsoft Fabric’s unified data lake.

4. What is Lakehouse</br>
- Exploring the hybrid data storage and analytics architecture.

5. What is Warehouse</br>
- Explanation of the compute layer used for querying data.

6. Why We Need Domains</br>
- Importance of domains for managing data access and governance.

7. Admin Portal Overview</br>
- Managing settings and resources through the Fabric admin portal.

8. How to Create a Workspace</br>
- Step-by-step process of setting up a workspace in Fabric.

---

## 📅 Week 2

### Class 3: Explore Lakehouse in Microsoft Fabric
1. Worked with SQL Query Editor using T-SQL
- Querying Lakehouse tables via SQL Analytics Endpoint

2. Used Notebook in Microsoft Fabric
- Running T-SQL queries interactively and viewing results

3. Explored Lakehouse Structure
- Accessed schemas and tables like fact_sale and dimension_stock_item

**Notebook Link:** [click here](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/TSQL/FILES/Lakehouse%20T-SQL.ipynb)

---

### Class 4: Explore Lakehouse with Spark
Practiced Spark SQL queries in a notebook connected to a Lakehouse.

**Notebook Link:** [click here](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SPARK%20SQL/Spark%20SQL%20Notebook.ipynb)


---

## 📅 Week 3

### Class 5: Explore Warehouse in Microsoft Fabric  
Practiced T-SQL Queries in Notebook (Connected to Warehouse)

**Notebook Link:** [click here](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/TSQL/FILES/Notebook%201.ipynb)

---

### Class 6: Explore Data Factory – Dataflow Gen2

## 🧪 Exercise 01 – Data Landing and Loading with Dataflow Gen2

This exercise covers loading data from a single Web API source and managing it across storage destinations in Microsoft Fabric, with transformations.

| Task                                      | Description                                               | Link                                                       |
|-------------------------------------------|-----------------------------------------------------------|------------------------------------------------------------|
| 1.1 Load Data via Web API                   | Load datasets from GitHub raw links using Web API         | [Exercise 1.1 - Data Loading](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING)             |
| 1.2 Transform and Load Data into Warehouse  | Transform and load the `Sales` dataset into the Warehouse | [Exercise 1.2 - Warehouse Destination](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION)   |
| 1.3 Landing Data into Lakehouse Storage     | Store `Items`, `Customers`, and `Geography` datasets in the Lakehouse for further use | [Exercise 1.3 - Lakehouse Destination](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION) |
---

## 🧪 Exercise 02 – Power Query Transformations

This section documents various data transformation techniques using **Power Query** in Microsoft Fabric.

### Transformation Tasks

| Task               | Link               |
|--------------------|--------------------|
| Pivot              | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/PIVOT)   |
| Unpivot            | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/UNPIVOT)   |
| Gap Filling        | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/GAP)   |
| Combine & Split    | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/COMBINE_SPLIT)   |
| Transpose          | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/TRANSPOSE)   |
| Replace Values     | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE)   |
| Joins              | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS)   |
| Append Queries     | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/APPEND_QUERIES)   |
| Date and Time      | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME)   |

---

## 📅 Week 4

### Class 7: Explore Data Pipeline in Microsoft Fabric  
- Creating Pipeline using Dataflow Gen2
- Creating and naming a new pipeline
- Adding pipeline activities and configuring Copy Data Assistant
- Connecting to HTTP data source (GitHub raw Excel)
- Configuring Excel file format and previewing data
- Selecting OneLake Lakehouse as destination and defining load settings
- Mapping data types at destination
- Validating and running the pipeline
- Adding Dataflow activity and setting execution order
- Setting up failure notifications via Outlook
- Scheduling pipeline runs for automation

**README FILE:** [click here](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/PIPELINE)

---

### Class 8: Working with Notebooks and PySpark  
- Introduction to notebooks in Microsoft Fabric  
- Creating and using notebooks within a Lakehouse  
- Loading data from Lakehouse tables into PySpark DataFrames  
- Performing transformations and analysis using PySpark  
- Demonstrated different types of joins using PySpark:
  - Inner Join  
  - Left Join  
  - Right Join  
  - Full Outer Join
  - Left Anti Join
  - Full join
  - cross join
- Filtering, selecting columns, Dropping columns, and aggregating data using PySpark
- Calculating Gross Sales, COGS, Discount using withColumn
- Saving Dataframe as delta table in pyspark
- Saving a DataFrame as a delta Table in Overwrite Mode

**Notebook Link:** [click here](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PYSPARK/PYSPARK_CMDS.ipynb)

---

## 📅 Week 5

### Class 9: Working with Direct Lake Semantic Model
- Workspace creation in Fabric  
- Lakehouse setup with Master and Fact schemas  
- Creating table shortcuts from Lakehouse and Warehouse  
- Configuring a semantic model using Direct Lake  
- Creating and activating table relationships  
- Finalizing model for reporting
- Creating Report

---

### Class 10: 
