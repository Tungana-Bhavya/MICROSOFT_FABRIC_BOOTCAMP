Landing Data into Microsoft Fabric Lakehouse Using Dataflow Gen2

This document provides a step-by-step guide to load and configure source data tables into Microsoft Fabric Lakehouse using Dataflow Gen2.

---

## Steps

### Step 1: Open Workspace
Navigate to the target Workspace in Microsoft Fabric where the Dataflow will be created or accessed.

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/DATA_LOADING/IMAGES/2_SELECT_DATAFLOWGEN2.jpg)

---

### Step 2: Load Data into Dataflow Gen2
- Create a new Dataflow Gen2 or open an existing one.
- Load your source data (e.g., Excel, SQL, SharePoint).
- Ensure data loads without errors.

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_1.jpg)

---

### Step 3: Select the Item Table
- From the list of loaded queries, select the **Item** table for transformation and loading.

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_1.jpg)

---

### Step 4: Add Data Destination for Item Table
- In the **Home** tab, select **Default Data Destination**.
- Click **Add** to start configuring the destination.

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_2.jpg)

---

### Step 5: Connect to Data Destination for Item Table
- Select the Lakehouse connection (e.g., Lakehouse01).
- Enter a Connection Name.
- Set Data Gateway to `none`.
- Choose Authentication Kind as `Organizational account`.
- Verify logged-in account.
- Click **Next**.

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_3.jpg)

---

### Step 6: Choose Lakehouse and Table Name
- Select the Lakehouse target (e.g., Laketbhavya0541).
- Enter the table name as `Git_Item`.
- Click **Next**.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_4.jpg)

---

### Step 7: Configure Destination Settings
- Enable **Use Automatic Settings**.
- Click **Save Settings**.

![Step 7](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_5.jpg)

---

### Step 8: Confirm Item Table Loaded
- The Item table is added successfully to the Lakehouse destination.

![Step 8](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_ITEM_TO_LAKEHOUSE_6.jpg)

---

### Step 9: Select Customer Table
- Select the **Customer** query.
- In **Properties**, click **+ Data Destination**.
- Choose **Lakehouse** as the destination.

![Step 9](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/CUSTOMER_1.jpg)

---

### Step 10: Connect to Data Destination for Customer
- Repeat Step 5 connection process.
- Click **Next**.

![Step 10](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/CUSTOMER_2.jpg)

---

### Step 11: Choose Lakehouse and Table Name for Customer
- Select Lakehouse target.
- Enter table name as `Git_Customer`.
- Click **Next**.

![Step 11](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/CUSTOMER_3.jpg)

---

### Step 12: Configure Destination Settings for Customer
- Enable **Use Automatic Settings**.
- Click **Save Settings**.

![Step 12](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/CUSTOMER_4.jpg)

---

### Step 13: Confirm Customer Table Loaded
- Customer table is added successfully to the Lakehouse destination.

![Step 13](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/CUSTOMER_5.jpg)

---

### Step 14: Add Geography Table to Destination
- Select the **Geography** query.
- In **Properties**, click **+ Data Destination**.
- Choose **Lakehouse** as the destination.

![Step 14](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_GEOGRAPHY_1.jpg)

---

### Step 15: Connect to Data Destination for Geography
- Repeat Step 5 connection process.
- Click **Next**.

![Step 15](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_GEOGRAPHY_2.jpg)

----

### Step 16: Choose Lakehouse and Table Name for Customer
- Select Lakehouse target.
- Enter table name as `Git_Geography`.
- Click **Next**.

![Step 16](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_GEOGRAPHY_4.jpg)

---

### Step 17: Configure Destination Settings for Geography
- Enable **Use Automatic Settings**.
- Click **Save Settings**.

![Step 17](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_GEOGRAPHY_5.jpg)

----

### Step 18: Confirm Geography Table Loaded
- Geography table is added successfully to the Lakehouse destination.

![Step 18](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/WEBAPI_DATAFLOW/LAKEHOUSE_DESTINATION/IMAGES/DATAFLOWGEN2_GEOGRAPHY_6.jpg)


----

### Key Points
- This guide covers the end-to-end process for loading data into Microsoft Fabric Lakehouse using Dataflow Gen2.  
- Following these steps ensures consistent and reliable data ingestion.  
- Proper configuration enables effective semantic modeling and analytics.  
- Adherence to naming conventions and authentication standards is essential.  

---
