# Microsoft Fabric Bootcamp – Dataflow Gen2 Pipeline Setup

This documents the process of creating a Dataflow Gen2 pipeline in Microsoft Fabric to ingest retail data from a  GitHub source into a Lakehouse.

---

## Steps


### Step 1: Open Workspace and Create a New Pipeline  
Go to your **Workspace**, click **+ New item**. 

![Step 1](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/1.jpg)

---

### Step 2: Search and Select Pipeline  
In the item selection dialog, search for and select **Pipeline** under the *Get Data* section. 

![Step 2](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/2.jpg)

---

### Step 3: Name and Create the Pipeline  
Provide a name for the pipeline (e.g., `Git_Retail_Data`) and click **Create**. 

![Step 3](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/3.jpg)

---

### Step 4: Pipeline Interface Overview  
The pipeline canvas opens, showing options like **Activities**, **Copy Data Assistant**, **Practice with Sample Data**, and **Templates**.  

![Step 4](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/4.jpg)

---

### Step 5,6: Launch Copy Data Assistant  and Select HTTP as Data Source  
Click **Copy Data Assistant** to start a guided data copy setup. </br>
Under **Choose Data Source**, use the search bar to find and select **HTTP**.  

![Step 5](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/5.jpg)

---

### Step 7: Enter Connection Details  
- **URL**: Paste the raw GitHub Excel file link  
- **Connection Name**: e.g., `Git Retail Data`  
- **Gateway**: None  
- **Authentication Type**: Anonymous  
- **Privacy Level**: None  
Click **Next**.

![Step 6](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/6.jpg)


---

### Step 8: Configure Request  
- **Request Method**: `GET`  
Click **Next**.

![Step 8](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/7.jpg)

---

### Step 9: File Format Configuration  
- **File Format**: Excel  
- **Worksheet Mode**: Index  
- **Sheet Index**: `0`  
- Enable: **First row as headers**  
Click **Next**.

![Step 9](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/8.jpg)

---

### Step 10: Preview the Data  
Click **Preview** to inspect the data and ensure it's loading correctly.  
Click **Next**.  

![Step 10](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/9.jpg)

---

### Step 11: Choose Data Destination – OneLake  
In the **OneLake Catalog**, select the Lakehouse (e.g., `Laketbhavya0541`).  

![Step 11](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/10.jpg)

---

### Step 12: Configure Load Settings  
- **Destination Folder**: `Tables`  
- **Load To**: New Table  
- **Table Name**: `Retail_Data`  
Click **Next**.

![Step 12](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/11.jpg)

---

### Step 13: Review and Save  
- Uncheck the box for **Start data transfer immediately**  
- Click **Save**

![Step 13](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/12.jpg)

---

### Step 14: View Pipeline Activity  
The new **Copy Data** activity is added to the pipeline canvas.  

![Step 14](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/13.jpg)

---

### Step 15: Rename the Activity  
Click on the activity and rename it to `Get Retail Data`. 

![Step 15](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/14.jpg)

---

### Step 16: Review Source Configuration  
Confirm that connection details, file format, worksheet mode, and sheet index are correctly set. 

![Step 16](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/15.jpg)

---

### Step 17: Review Destination Settings  
- **Destination Table**: `Retail_Data`  
- **Table Action**: Overwrite existing data

![Step 17](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/16.jpg)

---

### Step 18: Open Column Mapping  
Go to the **Mapping** tab to configure field mappings.  

![Step 18](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/17.jpg)

---

### Step 19: Modify Column Data Types  
Update the destination column data types as follows:  
- `OrderDate`: Date  
- `ItemID`: Integer  
- `UnitPrice`: Decimal  
- `Quantity`: Decimal  
- `Percentage`: Decimal  
- `LocationId`: Integer  
- `CustomerId`: Integer

![Step 19](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/18.jpg)

---

### Step 20: Save Mapping Changes  
Save the updated data type mappings. 

![Step 20](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/19.jpg)

---

### Step 21: Validate the Pipeline  
Click **Validate** from the **Home** tab to check for configuration issues.  

![Step 21](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/20.jpg)

---

### Step 22: Run the Pipeline  
After validation succeeds, click **Run** to execute the pipeline.  

![Step 22](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/21.jpg)

The pipeline will run successfully if configured correctly, as indicated by the success message and status.

![Step 23](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/22.jpg)

---

### Step 23: Add a Dataflow Activity  
From the **Activities** pane, drag a **Dataflow** activity to the pipeline canvas.  

![Step 24](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/23.jpg)

---

### Step 24: Set Pipeline Dependency  
Configure the **Dataflow** activity to run **after success** of the `Get Retail Data` activity.  

![Step 25](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/24.jpg)

---

### Step 25: Configure the Dataflow  
In the settings panel, select the target Dataflow: `LOAD_SALES_DATA`.  

![Step 25](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/25.jpg)


---

### Step 26: Add Outlook Notification (Optional)  
- From **Activities**, add **Outlook** activity

![Step 26](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/25.jpg)

  
![Step 26](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/26.jpg)

- Customize the failure message
  
![Step 26](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/27.jpg)

- Set recipient email  
- Click **Save**

![Step 26](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/28.jpg)

---

### Step 27: Open Schedule Configuration  
Go to the **Run** tab and click **Schedule** to configure pipeline execution timing.  

![Step 26](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/29.jpg)

---

### Step 28: Set Recurrence  
Define schedule frequency (e.g., daily, weekly) and execution time.  

![Step 28](https://github.com/Tungana-Bhavya/MICROSOFT_FABRIC_BOOTCAMP/blob/main/DATAFLOWGEN2/PIPELINE/FILES/30.jpg)
---

### Step 29: Final Pipeline View  
Pipeline is complete with **Copy Data**, **Dataflow**, **Outlook notification**, and **Scheduling**. 


---
  
## ✅ Output Summary

- Retail Excel data from GitHub is loaded into Lakehouse table `Retail_Data`.
- Dataflow `LOAD_SALES_DATA` runs on success.
- Outlook notification configured for failure scenarios.
- Learned how to schedule pipeline runs for automated execution.




