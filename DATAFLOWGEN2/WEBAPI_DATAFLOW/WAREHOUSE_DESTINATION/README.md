# Sales Data Integration using Dataflow Gen2 & Microsoft Fabric Warehouse

This document outlines the step-by-step process for transforming and loading **Sales data** into a **Microsoft Fabric Warehouse** using **Dataflow Gen2**.

---

## Prerequisites

Before starting, ensure you have:

- Access to Microsoft Fabric Workspace
- Permissions to create and run Dataflow Gen2
- A Microsoft Fabric Warehouse instance
- Organizational account credentials

## Step-by-Step Implementation

### Step 1: Open Workspace

- Navigate to the target **Workspace** in Microsoft Fabric where your dataflow will be created or accessed.

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/1_WORKSPACE_NEW_ITEM.jpg)

---

### Step 2: Load Data into Dataflow Gen2

- Create a **new Dataflow Gen2**, or open an existing one.
- Load your **source data** into the dataflow (e.g., from Excel, SQL, SharePoint, etc.).
- Ensure the data loads without errors.

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_1.jpg)

---

## Step 3: Select the Sales Table

- From the list of loaded queries, select the **Sales** table.
- This table will be used for transformation and loading.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S1.jpg)

---

## Step 4: Create a Custom Column – GrossAmount

- Go to the **Add Column** tab.
- Click on **Custom Column**.
- Enter the formula below to calculate the gross amount:
  ```powerquery
  =[Qty] * [Price]
- Click **Ok** to create column

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S2.jpg)

---

## Step 5: GrossAmount Column Added

A new column named GrossAmount is added to the Sales query.

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S3.jpg)

---

## Step 6: Add Data Destination

From the Home tab, select Default Destination -> Add Destination.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S4.jpg)

---

## Step 7: Choose Data Destination Type

In the Choose Data Destination panel, select Microsoft Fabric Warehouse from the available options.

![Step 7](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S5.jpg)

---

## Step 8: Configure Connection Settings

In the Connect to Data Destination step:

- Create a new connection
- Set Connection Name to Warehouse_tbhavya0541
- Gateway: None
- Authentication Kind: Organizational Account
- Click Next to continue.

![Step 8](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S7.jpg)

---

## Step 9: Choose Warehouse and Table

Select the target Warehouse, and enter the table name as Git_Sales and Click Next.

![Step 9](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S8.jpg)

---

## Step 10: Configure Load Settings

In the Destination Settings panel:

- Load Method: Replace
- Schema: Fixed Schema
- Verify column mapping, then click on Save Settings.

![Step 10](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S9.jpg)

---

## Step 11: Sales Data Added to Warehouse

The transformed Sales query is now configured to load into the warehouse.

![Step 11](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S10.jpg)

---

## Step 12: Save and Run the Dataflow

From the Home tab, click Save to preserve changes, and then run the dataflow to load the data into the warehouse.

![Step 12](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/WAREHOUSE_DESTINATION/IMAGES/S11.jpg)


## Output Summary

- Created a custom column (GrossAmount) using calculated values.
- Connected Dataflow Gen2 to Microsoft Fabric Warehouse.
- Configured data destination with appropriate schema and settings.
- Successfully loaded Sales query into the warehouse table Git_Sales.

