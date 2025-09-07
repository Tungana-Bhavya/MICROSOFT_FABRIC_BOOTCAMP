# Replace Transformation using Power Query in Dataflow Gen2 (Microsoft Fabric)


This document shows how to clean and fix data by replacing values and handling blanks using Power Query in Dataflow Gen2 in Microsoft Fabric.

### Implementation Steps
### Step 1: Select the Query

- Open Power Query Editor in Dataflow Gen2.
- Select the query named Replace.
  
![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_1.jpg)

---

### Step 2: Promote Headers and Rename Columns

- From the Transform tab, click Use First Row as Headers.
- Rename columns as needed (e.g., Item, Item Cat).
- Change the column data types to Text.
  
![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_2.jpg)

---

### Step 3: Select Replace Values

- Select the columns (Item and Item Cat).
- Click Replace Values in the Transform tab.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_3.jpg)

---

### Step 4: Replace “GG” with “Good”

- Find GG and replace it with Good.
- Ensure Match entire cell contents is checked.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_4.jpg)

  
### Step 5: Replace Null Values with “NA”

- Use Replace Values again on the selected columns.
- Find null and replace with NA.

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_5.jpg)

---

### Step 6: Replace Dash (“-”) with “NA”

- Use Replace Values once more.
- Find - and replace with NA.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_6.jpg)

---

### Step 7: Review and Save

- Verify that all replacements have been applied correctly.
- Save and close the query.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/REPLACE/IMAGES/REPLACE_8.jpg)

---

### Key Learnings

- Promoting the first row as headers makes the column names clear and meaningful.
- Replacing specific values like GG with Good.
- Handling nulls and placeholder values like - improves data quality.
- Power Query in Dataflow Gen2 provides a simple way to clean and transform data within Microsoft Fabric.

---
