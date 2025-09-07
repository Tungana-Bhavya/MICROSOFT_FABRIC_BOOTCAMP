# Microsoft Fabric Power Query : Joins (Fabric Dataflow Gen2)

This guide demonstrates how to perform differnt **Joins** between two queries (master and Details) in Power Query within Fabric Dataflow Gen2.

## Step-by-Step Implementation:
## Inner Join in Power Query (Fabric – Dataflow Gen2)
### Step 1: Display the Details Table

- In the Queries pane, select the query named `Details`.
- This displays the Details table with columns like **ID**, **Cat ID**, and **Name**.

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/1_DETAILS_TABLE.jpg)

---

### Step 2: Display the master Table

- Select the query named `master` from the Queries pane.
- The master table contains columns like **Category ID** and **Name**.

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/2_MASTER_TABLE.jpg)

---

### Step 3: Open Merge Dialog

- Click on “Home” -> “Merge Queries”.
In the Merge window:
- Select `master` as the Left table.
- Select `Details` as the Right table.
- Match **Category ID** from master with **Cat ID** from Details.
- The system confirms: "The selection matches 4 rows from both the tables."

![step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/INNER_JOIN_MERGE_TABLE_WITH_KEYS_1.jpg)

---

### Step 4: Choose Join Type - Inner Join

In the same merge window:
- Select `Inner Join` under the Join kind options.
- This will keep only matching rows from both tables.

![step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/INNER_JOIN_SELECT_INNER_JOIN_2.jpg)

---

### Step 5: Apply the Merge

- After choosing Inner Join, click **Ok**.
- A new column named Details will appear containing nested tables.

![step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/INNER_JOIN_RENAME_TABLE_AS_INNER_JOIN_3.jpg)

---

### Step 6: Expand the Details Table

- Click the expand icon (🔽) next to the `Details` column.
- Select all the columns to expand: **ID, Cat ID, and Name**.
- Uncheck **Use original column name as prefix** for cleaner column names.
- Click OK.

![step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/INNER_JOIN_RESULT_5.jpg)

The Inner Join between `master` and `Details` queries was successfully performed. Only the matching rows from both tables are included in the final result.

---

## Left Join in Power Query (Fabric – Dataflow Gen2)
Perform a Left Outer Join between master and Details tables.

### Step 1: Merge Queries Using Left Outer Join

From the master query:
- Go to **Home** > **Combine** > **Merge Queries**
- In the Merge dialog:
   - Select `Details` as the right table
   - Match **Category ID** from master with **Cat ID** from `Details`
   - Choose Join kind: **Left outer**
- Click OK

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/LEFT_JOIN_1.jpg)

---

### Step 2: Expand the Merged Table

After merging:
- Click the expand icon next to the Details column
- Select: **ID, Cat ID, and Name**
- Click **OK** to expand and apply

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/LEFT_JOIN_2_RESULT.jpg)


The Left Join is successfully applied — unmatched rows from master are retained with null values from Details.

---

## Right Join in Power Query (Fabric – Dataflow Gen2)
Perform a right outer join between master and details table.

### Step 1: Perform the Right Join

- In Power Query, select your Left Table — this is the main table you're working with.
- Click **Home** -> **Merge** Queries.
- In the merge window, choose Details as the Right Table to merge with.
- Select the matching column(s), e.g., Category ID, in both tables.
- Under Join kind, select Right outer.
- Click **OK**.
The selection matches 6 of 7 rows from the second table.

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/RIGHT_JOIN_1.jpg)

---

### Step 2: Expand the Joined Table

- Click the expand icon next to the new column (which holds the `Details` table).
- Select the fields you want to bring in (e.g., ID, Cat ID, Name).
- Click **OK** to finalize the join.

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/RIGHT_JOIN_RESULT_2.jpg)

The Right Join is successfully applied — unmatched rows from the Details table (Right Table) are retained with null values from the Left Table.

---

## Full Join in Power Query (Fabric – Dataflow Gen2)

### Tables
- **Left Table:** `master`
- **Right Table:** `Details`

### Step 1:

- Go to `Home` → `Merge Queries`.
- In the Merge window:
   - Select `master` as left table.
   - Select `Details` as right table.
   - Match on `Category ID` ↔ `Cat ID`.
   - Choose **Join kind:** `Full outer`.
   - Click `OK`.
*Matches: 4 of 6 rows from both tables*

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/FULL_JOIN_1.jpg)

### Step 2:

- Expand the merged `Details` column:
   - Select: `ID`, `Cat ID`, `Name`
   - Click `OK`.

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/FULL_JOIN_RESULT_2.jpg)

All rows from both tables are successfully included. Non-matching rows are filled with `null` values.

---

## Left Anti Join in Power Query (Fabric – Dataflow Gen2)

### Tables
- **Left table:** `master`
- **Right table:** `Details`

### Step 1: Merge Settings (Left Anti Join)

- selected Details as the right table
- Join kind: **Left Anti Join**
- Power Query reports:
“The selection returns 1 of 5 rows from the first table”

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/LEFT_ANTI_JOIN_1.jpg)

---

### Step 2: Result After Expanding

- Only **unmatched rows** from the `master` table are retained
- **No matching rows** from `Details` are included

The Left Anti Join is successfully applied — unmatched rows from the left table (master) are returned, and no columns from the right table (Details) are included.

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/LEFT_ANTI_JOIN_RESULT_2.jpg)

---

## Right Anti Join in Power Query (Fabric – Dataflow Gen2)

### Tables
- **Left table:** `master`
- **Right table:** `Details`

### Step 1: Merge Settings (Right Anti Join)

- Selected `Details` as the right table
- Join kind: **Right Anti Join**
- Power Query reports:
“The selection returns 1 of 7 rows from the second table”

![step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/RIGHT_ANTI_JOIN_1.jpg)

---

### Step 2: Result After Expanding

- Only **unmatched rows** from the Details table are retained
- No matching rows from `master` are included

![step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/POWER_QUERY_EXERCISE/JOINS/IMAGES/RIGHT_ANTI_JOIN_RESULT_2.jpg)


The Right Anti Join is successfully applied — unmatched rows from the right table (Details) are returned, and no columns from the left table (master) are included.


### Key Points:

- Inner Join → Only matching rows from both tables
- Left Join → All rows from left, unmatched right rows show null
- Right Join → All rows from right, unmatched left rows show null
- Full Join → All rows from both tables, unmatched rows show null
- Left Anti Join → Rows from left table with no match in right
- Right Anti Join → Rows from right table with no match in left

---
