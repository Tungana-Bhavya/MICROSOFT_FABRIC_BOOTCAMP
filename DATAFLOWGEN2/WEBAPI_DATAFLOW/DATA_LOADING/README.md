# Data Loading via Web API in Dataflow Gen2  

This document describes the process of loading data into Microsoft Fabric using the **Web API connector** in **Dataflow Gen2**. Data from a GitHub Excel file was ingested, including multiple tables: `Customer`, `Geography`, `Item`, and `Sales`.

## Step-by-Step Implementation

### Step 1: Open Workspace

Navigate to the desired Workspace in Microsoft Fabric.

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/1_WORKSPACE_NEW_ITEM.jpg)

---

### Step 2: Create New Data Item

Click on + New Item, then select Dataflow Gen2 from the available options.

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/2_SELECT_DATAFLOWGEN2.jpg)

---


### Step 3: Name the Dataflow

Enter a name such as `LOAD_SALES_DATA` and click **Create** to open the editor.

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/3__NAMING_DATAFLOWGEN2.jpg)

---

### Step 4: Dataflow Interface Overview

The interface offers multiple options to add data, such as Excel, SQL Server, Text/CSV, Dataflows, Power Query templates, and Web APIs.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/4_WORKFLOW_GEN2.jpg)

---

### Step 5: Access Data Sources

Go to the **Home** tab, click **Get Data**, then select **More** to see all connectors.

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/5_GET_DATA.jpg)

---

### Step 6: Select Web API as Data Source

Search for and choose the **Web API** connector.

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/6_WEB_API_SOURCE.jpg)

---

### Step 7: Connect to GitHub Source

Configure the Web API connection by providing:
- The **GitHub raw URL** for the Excel data  
- A **Connection Name**  
- Gateway: set to `None`  
- Authentication: set to `Anonymous`  
- Privacy Level: set to `None`  
Click **Next** to continue.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/7_URL.jpg)

---

### Step 8: Select Tables to Load

From the detected tables, select:
- `Customer`  
- `Geography`  
- `Item`  
- `Sales`  
Click **Create** to load.

![Step 7](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/8_CHOOSE_DATA.jpg)

---

### Step 9: Confirm Data Loaded

The selected tables are successfully loaded into the Dataflow Gen2 canvas and are ready for further processing.

![Step 8](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_1.jpg)


---

## Output Summary

- Successfully connected to external GitHub Excel file via **Web API**  
- Loaded four datasets (`Customer`, `Geography`, `Item`, `Sales`) into **Dataflow Gen2**  
- Data is prepared for transformation or downstream analytics  

---


