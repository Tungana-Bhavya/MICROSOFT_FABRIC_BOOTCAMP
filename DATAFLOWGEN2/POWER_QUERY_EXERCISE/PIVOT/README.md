# Unpivot Transformation

This exercise demonstrates how to perform the **Unpivot** operation using Power Query in Dataflow Gen2, after loading data via Web API.

---

## Steps

### Step 1: Load Data  
Load the dataset from the Web API source into Dataflow Gen2.

![Step 1: Load Data](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/PIVOT/IMAGES/PIVOT_1.jpg)

---

### Step 2: Apply Unpivot Other Columns  
In the Transform tab, select **Unpivot Other Columns** to reshape the data.

![Step 2: Unpivot Other Columns](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/PIVOT/IMAGES/PIVOT_2.jpg)

---

### Step 3: Rename Columns  
Rename the `Attribute` column to **Subjects**.

![Step 3: Rename Attribute to Subjects](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/PIVOT/IMAGES/PIVOT_3.jpg)

---

### Step 4: Rename Value Column  
Rename the `Value` column to **Marks**.

![Step 4: Rename Value to Marks](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/PIVOT/IMAGES/PIVOT_4.jpg)

---

## Key Points 
- Unpivoting converts wide-format data into a normalized long-format, making it easier to analyze.
- Column renaming improves readability and understanding of the dataset.
