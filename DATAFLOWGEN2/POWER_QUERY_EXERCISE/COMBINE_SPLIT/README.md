# Combine Split in Microsoft Fabric Dataflow Gen2 (Power Query)

This document provides a step-by-step guide to split a column by delimiter and transform the data within **Power Query** in **Microsoft Fabric Dataflow Gen2**.

---

## Steps

### Step 1: Load Source Data  
- A query contains a column with combined values separated by commas.

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/COMBINE_SPLIT/IMAGES/COMBINE_SPLIT_1.jpg)

---

### Step 2: Split Column by Delimiter  
- Navigate to the **Add Column** tab.  
- Select **Split column** → **By delimiter**.  
- Choose the delimiter (e.g., comma `,`).  
- Access **Advanced** options.  
- Under **Split at**, select **Each occurrence of the delimiter**.  
- Under **Split into**, select **Rows**.  
- Confirm by clicking **OK**.


![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/COMBINE_SPLIT/IMAGES/COMBINE_SPLIT_2.jpg)

---

### Step 3: Promote First Row as Headers  
- Go to the **Transform** tab.  
- Select **Use first row as headers** to promote the first row to column headers.
- Change the data types of columns as necessary (e.g., `Name` as text, `Rank` as text).  


![step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/COMBINE_SPLIT/IMAGES/COMBINE_SPLIT_3.jpg)

---

### Step 4: Splitting Column
- When splitting the column by delimiter:  
  - From **Advanced options**, select **Comma (,)** as the delimiter.  
  - Under **Split at**, choose **Each occurrence of the delimiter**.  
  - Under **Split into**, select **Rows**.  
  - For **Quote character**, select **-** (none).  
- Confirm changes by clicking **OK**.

![step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/COMBINE_SPLIT/IMAGES/COMBINE_SPLIT_4.jpg)

---

## Key Points  
- Splitting the column by delimiter separates combined values into individual rows.  
- Splitting into **rows** normalizes the data structure.  
- Promoting the first row as headers ensures proper column names.  
- Changing data types maintains data accuracy for analysis.

---
