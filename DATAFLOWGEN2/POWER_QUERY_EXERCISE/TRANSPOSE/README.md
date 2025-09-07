# Transpose Data using Power Query (Dataflow Gen2)

This documents explains how to  **transpose a table** using **Power Query** in **Dataflow Gen2** (Microsoft Fabric). Transposing switches rows and columns, which is useful for reshaping data to fit your reporting or modeling needs.

---

##  Transformation Steps

### step 1: Select the Query

- Open the **Power Query Editor** in your Dataflow Gen2 workspace.
- In the Queries pane, select the dataset you want to transpose (e.g., `Transpose`).

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/TRANSPOSE/IMAGES/TRANSPOSE_1.jpg)

---

### Step 2: Apply Transpose

- With the table selected:
  - Go to the **Transform** tab.
  - Click **Transpose** to rotate the data layout.
    
![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/TRANSPOSE/IMAGES/TRANSPOSE_2.jpg)

---

### Step 3: Use First Row as Headers

- After transposing:
  - Stay in the **Transform** tab.
  - Click **Use First Row as Headers** to promote the first row as the column headers.

---

### Step 4: Rename Columns

- Use the **Rename Columns** option to provide meaningful names.
  - For example, if the transposed column represents dates, rename `Measure` to `Date`.

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/TRANSPOSE/IMAGES/TRANSPOSE_4.jpg)

---

## Key Points

- Transposing flips the data layout: rows become columns.
- Use **"Use First Row as Headers"** immediately after transposing to structure your table correctly.
- Renaming columns improves clarity and makes the dataset more readable.
- These transformations are done within **Power Query (M)** in **Microsoft Fabric Dataflow Gen2**.
- Always validate the output to ensure it fits your reporting or modeling needs.

---
