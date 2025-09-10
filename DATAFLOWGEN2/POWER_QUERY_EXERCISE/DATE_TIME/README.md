# Datetime Transformations in Microsoft Fabric – Dataflow Gen2 (Power Query) 

---

## Steps

### Step 1: Load Data  
- Load data into Dataflow Gen2 from a source (e.g., Web API, file, database).  
- Select the `Datetime` query from the **Queries pane**.

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_1.jpg)

---

### Step 2: Set Datatype for Datetime Column  
- In the **Transform** tab, set the `Datetime` column to **Date/Time** type.

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_2.jpg)

---

### Step 3: Insert Year Column  
- Go to **Add Column → Date → Year → Year**  
- Adds a column with the year extracted.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_3.jpg)

---

### Step 4: Insert Month Column  
- Go to **Add Column → Date → Month → Month**  
- Adds the month number (1–12).

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_4.jpg)

---

### Step 5: Insert Days in Month and Week of Month  
- Add **Days in month**: **Add Column → Date → Days in month**  
- Add **Week of month**: **Add Column → Date → Week → Week of month**

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_5.jpg)

---

### Step 6: Insert Time Component  
- Go to **Add Column → Time → Time only**  
- Adds a column with just the time part.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_5.jpg)

---

### Step 7: Insert Date Component and Reorder Columns
- Go to **Add Column → Date → Date only**  
- Adds a column with just the date part.

- Go to **Home → Manage Columns → Reorder Columns**  
- order:  
  `Datetime`, `Date`, `Year`, `Month`, `Days in month`, `Week of month`, `Time`


![Step 7](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/DATE_TIME/DATE_TIME_6.jpg)

---

## Key Points

- Set the correct data type first.  
- Break datetime into parts for easier analysis.  
- Separate date and time for flexibility.  
- Reorder columns to keep data organized.

---
