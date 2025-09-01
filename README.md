# MICROSOFT FABRIC BOOTCAMP – LEARNING JOURNEY

This repository documents hands-on exercises completed during the Microsoft Fabric Bootcamp. It covers key concepts such as Lakehouse, Warehouse, Data Pipelines, and practical experience with Dataflow Gen2 and Power Query transformations within Microsoft Fabric.

---

## 📅 Week 1

### Class 1: Introduction to Microsoft Fabric
- What is Microsoft Fabric?
- Key Features of Microsoft Fabric
- Overview of OneLakehouse architecture
- Microsoft Fabric components and ecosystem
- What is a Lakehouse?
- What is a Warehouse?
- Use cases and business value

### Class 2: Workspace and Lakehouse Concepts
- Understanding Workspaces
- Introduction to Lakehouse architecture

---

## 📅 Week 2

### Class 3: Explore Lakehouse in Microsoft Fabric  
### Class 4: Explore Lakehouse with Spark

---

## 📅 Week 3

### Class 5: Explore Warehouse in Microsoft Fabric  

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

| Task               | Description                                                   | Link               |
|--------------------|---------------------------------------------------------------|--------------------|
| Pivot              | Convert rows into columns based on a category or key          | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/PIVOT)   |
| Unpivot            | Convert columns into attribute-value rows                     | [View Details](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/tree/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/UNPIVOT)   |
| Gap Filling        | Fill down or fill up missing values in a column               | [View Details]()   |
| Combine & Split    | Combine multiple columns or split one column by delimiter     | [View Details]()   |
| Transpose          | Switch rows into columns or columns into rows                 | [View Details]()   |
| Replace Values     | Replace specific values within columns                        | [View Details]()   |
| Joins              | Merge tables using join types (Inner, Left, Right, etc.)      | [View Details]()   |
| Append Queries     | Stack multiple queries (tables) on top of each other          | [View Details]()   |
| Date and Time      | Extract or manipulate date and time components                | [View Details]()   |

---

## 📅 Week 4

### Class 7: Explore Data Pipeline in Microsoft Fabric  
- Creating and configuring pipelines  
- Adding pipeline activities
- Scheduling and monitoring pipeline runs
- 
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
  - Right Anti Join
  - Full join
- Filtering, selecting columns, and aggregating data using PySpark

## 📅 Week 5

### Class 9: Working with Direct Lake Semantic Model
- Creating Semantic Model
- Creating Report
  
### Class 10: 
