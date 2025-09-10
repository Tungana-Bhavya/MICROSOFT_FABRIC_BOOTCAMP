# Semantic Model Creation Using Lakehouse & Direct Lake – Microsoft Fabric (Dataflow Gen2)

## Overview  
This document provides the end-to-end process for creating a semantic model in **Microsoft Fabric**, using **Lakehouse-based schemas** and establishing relationships via **Direct Lake mode**. The workflow includes setting up a workspace, configuring a Lakehouse with table shortcuts, and generating a semantic model with defined relationships.

---

## Steps

### Step 1: Create a New Workspace  
Navigate to the **Workspaces** section and select **+ New workspace**.

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/1.jpg)

---

### Step 2: Configure Workspace  
Provide the workspace name as `0541_REPORTING` in the settings pane.  
Click **Apply** to initiate workspace creation.

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/2.jpg)

---

### Step 3: Open the Workspace  
Upon successful creation, the new workspace interface loads automatically.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/3.jpg)

---

### Step 4: Add a Lakehouse  
Click **+ Add new item** and select **Lakehouse** from the available item types.

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/4.jpg)

---

### Step 5: Configure the Lakehouse  
Enter the name `Reporting` for the new Lakehouse.  
Enable the **Lakehouse schemas** option and click **Create**.

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/5.jpg)

---

### Step 6: Add a New Schema  
In the **Explorer**, select the ellipsis (⋮) next to **Tables** and choose **New schema**.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/6.jpg)

---

### Step 7: Name the Schema  
Assign the name `Master` to the schema and click **Create**.

![Step 7](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/7.jpg)

---

### Step 8: Add Additional Schema  
Repeat the schema creation process to add a second schema named `Facts`.

![Step 8](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/8.jpg)

---

### Step 9: Create Table Shortcuts in Master Schema  
Right-click on the `Master` schema and select **New table shortcut**.

![Step 9](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/9.jpg)

---

### Step 10: Select Shortcut Source  
In the shortcut configuration window, choose **Microsoft OneLake – Fabric** as the source.

![Step 10](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/10.jpg)

---

### Step 11: Select Tables from Source Lakehouse  
Choose the source Lakehouse `laketbhavya0541`.
Click **Next** to proceed.

![Step 11a](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/12.jpg)

Also, select the following tables:  
- `Git_customer`  
- `Git_geography`  
- `Git_item`
Click **Next** to proceed.

![Step 11b](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/13.jpg)

---

### Step 12: Rename Shortcut Tables  
Update table names as follows:  
- `Git_customer` → `customer`  
- `Git_geography` → `geography`  
- `Git_item` → `item`

![Step 12](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/14.jpg)

---

### Step 13: Confirm Shortcut Table Creation  
Click **Create** to finalize table shortcut additions.

![Step 13](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/15.jpg)

---

### Step 14: Verify Tables in Master Schema  
The shortcut tables appear under the `Master` schema in the Lakehouse.

![Step 14](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/16.jpg)

---

### Step 15: Create Table Shortcut for Facts Schema  
Right-click on the `Facts` schema and choose **New table shortcut**.  

![Step 15](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/17.jpg)

Also, Select **Microsoft OneLake – Fabric** as the source.

![Step 16](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/18.jpg)

---

### Step 16: Select Source Warehouse  
Choose the Warehouse `WH01` and click **Next**.

![Step 16](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/19.jpg)

---

### Step 17: Select Table from Warehouse  
From the list of available tables, select `Git_sales` and click **Next**.

![Step 17](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/20.jpg)

---

### Step 18: Rename Fact Table  
Rename `Git_sales` to `sales` and click **Create**.

![Step 18](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/21.jpg)

---

### Step 19: Verify Fact Table Addition  
The `sales` table appears under the `Facts` schema.

![Step 19](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/22.jpg)

---

### Step 20: Create a Semantic Model  
From the Home interface, select **New Semantic Model**.  
In the configuration panel, select all available tables and click **Confirm**.

![Step 20](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/23.jpg)

---

### Step 21: Name the Semantic Model  
Enter `Sales_SM01` as the semantic model name and click **Next**.

![Step 21](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/25.jpg)

---

### Step 22: Open Semantic Model Interface  
The semantic model canvas loads, displaying all selected tables.

![Step 22](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/26.jpg)

---

### Step 23: Create Relationship (sales → item)  
Drag `ItemId` from the `sales` table to the `item` table.  

![Step 23](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/27.jpg)

Then, the system automatically detects a **many-to-one** relationship.  
Enable the **active relationship** checkbox and click **Save**.

![Step 23](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/28.jpg)

---

### Step 24: Relationship Confirmed (sales → item)  
The relationship is successfully established between `sales` and `item`.

![Step 24]([Step 23](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/29.jpg))

---

### Step 25: Create Relationship (geography → sales)  
Drag `CityId` from the `geography` table to the `sales` table.

![Step 25](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/30.jpg)

---

### Step 26: Confirm Relationship (geography → sales)  
A **one-to-many** relationship is detected.  
Enable the active status by checking the box and click **Save**.

![Step 26](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/31.jpg)

---

### Step 27: Create Relationship (sales → customer)  
Drag `CustomerId` from `sales` to `customer`.  
A **many-to-one** relationship is detected. Click **Save**.

![Step 27](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/32.jpg)

---

### Step 28: All Relationships Established  
All required relationships between fact and dimension tables are created successfully.

![Step 28](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/SEMANTIC_MODEL_AND_REPORTING/IMAGES/33.jpg)

---

## Key Points

- Workspaces organize assets like Lakehouses, tables, and semantic models.  
- Lakehouse schemas help group tables logically (e.g., `Master`, `Facts`).  
- Table shortcuts reference tables from other Lakehouses or Warehouses.  
- Semantic models enable relationships and support reporting tools.  
- Relationships auto-detect cardinality and can be activated in the model.  
- Direct Lake allows querying data without importing into memory.

---
