# How to Pivot Data using Power Query (Dataflow Gen2)

This exercise explains how to transform data using Power Query in Dataflow Gen2. The process involves applying a **Pivot** operation to reshape and summarize a dataset.

---

## Steps

### Step 1: Load Data  
Load data from a Web API source into Dataflow Gen2.  
The dataset `unpivot` includes three columns: `Month`, `Measure`, and `Value`.

![Step 1: Load Data](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/UNPIVOT/IMAGES/UNPIVOT_1.jpg)

---

### Step 2: Apply Pivot Transformation  
- Select both the `Measure` and `Value` columns.  
- Click on **Pivot Column** under the Transform tab.  
- In **Advanced Settings**, confirm `Measure` is set as the **pivot column** and `Value` as the **values column**.  
- Apply the **Sum** aggregation function to combine duplicate records grouped by `Month`.

This step generates separate columns such as `Sales` and `Margin`.

![Step 2: Pivot Settings](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/UNPIVOT/IMAGES/UNPIVOT_2.jpg)

---

### Step 3: Review the Result  
The final output shows a pivoted table with `Month`, `Sales`, and `Margin` columns.  
Values are aggregated using the **Sum** function.

![Step 3: Pivoted Output](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/UNPIVOT/IMAGES/UNPIVOT_3.jpg)

---
### Key Points
This transformation reshapes and summarizes the data, making it ready for analysis and reporting.
