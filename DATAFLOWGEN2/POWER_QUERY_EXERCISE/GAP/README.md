# Data Cleaning using Power Query (Dataflow Gen2)

This document explains how to clean and prepare data using **Power Query** in **Dataflow Gen2** (Microsoft Fabric). The process involves removing blank rows and duplicate entries to ensure the dataset is complete, accurate, and ready for reporting or modeling.

---

This dataset may contain blank rows or duplicate entries that need to be removed as part of the data preparation process.


## Transformation Steps

mn headers.

### Step 1 & 2: Select the Query and Promote Headers

- In the **Power Query Editor**, select the `Gap` query from the Queries pane on the left.

- Then, go to the **Transform** tab and click Use **First Row as Headers** to promote the first row as column headers.

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/GAP/IMAGES/GAP_5.jpg)

---

### Step 3: Remove Rows

- Return to the **Home** tab.
- From the **Reduce Rows** dropdown, click **Remove Rows**.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/GAP/IMAGES/GAP_3.jpg)

---

### Step 4: Remove Blank Rows

- Under the **Remove Rows** options, select **Remove Blank Rows** to eliminate any empty records from the dataset.

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/GAP/IMAGES/GAP_3.jpg)

---

### Step 5: Remove Duplicates

- Again, under **Reduce Rows**, select **Remove Duplicates**.
- This will remove duplicate entries across all columns or based on specific ones (like `Item`), depending on your selection.

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/GAP/IMAGES/GAP_4.jpg)

---

### Step 6: Data Cleaning Completed

- At this point:
  - Blank rows are removed 
  - Duplicates are eliminated 
  - Headers are promoted 

the  dataset is now clean and ready for use.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/GAP/IMAGES/GAP_1.jpg)

---

## Key Points

- **Promote headers first** before performing any row-based cleaning operations.
- Removing blank rows and duplicates ensures your data is consistent and analysis-ready.
- All operations are performed within **Power Query (M)** in **Microsoft Fabric Dataflow Gen2**.
- These steps are part of standard **data cleansing** best practices in any data project.
