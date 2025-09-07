# Appending Queries in Microsoft Fabric Dataflow Gen2 (Power Query)

## Overview
This document provides a step-by-step guide to append queries (combine rows from multiple tables) within **Power Query** in **Microsoft Fabric Dataflow Gen2**.

---

## Steps

### Step 1: Open Append Queries Menu
- In **Power Query Editor** of Microsoft Fabric Dataflow Gen2, navigate to the **Home** tab.
- Click on **Combine** dropdown.
- Select **Append queries** → **Append queries as new**.  
  *This creates a new query by appending selected queries without modifying the originals.*

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/APPEND_QUERIES/IMAGES/APPEND_QUERIES_1.jpg)

---

### Step 2: Configure Append Queries
- In the **Append** dialog box:
  - Choose **Two tables**.
  - Select the **First table** (e.g., `master`).
  - Select the **Second table** (e.g., `master (2)`).
- Click **OK** to proceed.

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/APPEND_QUERIES/IMAGES/APPEND_QUERIES_2.jpg)

---

### Step 3: Review Appended Data
- The new appended query will show combined rows from both tables stacked vertically.
- Check column names and data types to ensure consistency.

![step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/APPEND_QUERIES/IMAGES/APPEND_QUERIES_3.jpg)

---

### Step 4: Verify Query in Query List
- The new appended query appears in the list (e.g., named `Append`).
- Confirm that all rows from both source tables are present.

![step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/APPEND_QUERIES/IMAGES/APPEND_QUERIES_4.jpg)

---

### Step 5: Append Multiple Tables Using M Code (Optional)
- To append more than two tables, use the **M language** function `Table.Combine` in the formula bar:
  ```m
  Table.Combine({master, #"master (2)", master})

![step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/APPEND_QUERIES/IMAGES/APPEND_QUERIES_5.jpg)

---

### Key Points

- Append adds rows from one table below another.
- Use Append queries as new to keep original tables safe.
- You can add two or more tables together.
- For many tables, use the Table.Combine function.
- Always check your final table to make sure data is correct.
