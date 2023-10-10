## VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION
### Contents
1. Title
2. Tools Used
3. Description of Dataset
4. Importing Data & Combining Multiple CSV files
5. Filtering and Removing Duplicates
6. Handling Missing Values
7. Data Transformation
8. Removing Unnecessary Columns
9. Error Handling and Data Merging
10. Loading Cleaned Data into Excel/PowerBI for further analysis
----
### Tools Used
Microsoft Power Query Editor through MS-Excel/PowerBI

### Description of Dataset
The vehicle sales data has been collected from the <b>Regional Transport Authority Vehicle Online Sales Data</b> through a website https://data.telangana.gov.in/. The data between January 2023 to August 2023 were collected for performing data analysis and visualization using Business Intelligence Tool. The Excel files from January 2023 to August 2023 were combined using Microsoft Power Query Editor. The vehicle sales data consists of record_number, sl_no, modelDesc, fuel, color, vehicleClass, 
makeYear, seatCapacity, insuranceValidity, secondVehicle, tempRegistration, category, makerName, officecd, fromDate and toDate.

### Importing Data & Combining Multiple CSV files

The various csv files containing sales data for vehicles were kept together in a folder, from January 2023 to August 2023. The vehicle sales folder was loaded using power query editor.<br>

From Power Query tab, choose <b>From File</b> option, select <b>From Folder</b> options then type the folder path or browse the relevant 
folder from the dialog box.<br>
***Power Query -> From File -> From Folder -> Type or paste folder path or browse folder location -> Click Ok*** <br>

From Diaglog box, the required option such as ***Combine & Edit*** were selected as shown below.
<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_DATA_1_LOADING%20FILES.jpg">
</p>

After selecting ***Combine & Edit*** option, the dialog box appears as below:

<p align="center">
  <img  src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_DATA_2_COMBINE_FILES.jpg">
</p>

After Click on Ok button, the power query editor will automatically check and applies the correct data type for all the columns. This step is automatically recorded in the ***Applied Steps***. Sometimes the given data type for the columns may not be correct. Then, data type can be change by selecting the specific column and choosing the required data type from the ***Transform*** tab option.

### Filtering and Removing Duplicates

The vehicle sales data consists of 16 columns such as record_number, sl_no, modelDesc, fuel, color, vehicleClass, 
makeYear, seatCapacity, insuranceValidity, secondVehicle, tempRegistration, category, makerName, officecd, fromDate and toDate. From the vehicle sales data, 8 unwanted columns as record_number, sl_no, makeYear, seatCapacity, insuranceValidity, secondVehicle, officecd and toDate were removed by selecting all the columns and choosing ***Remove Columns*** from file menu or right clicking mouse on the one of the selected column and choose ***Remove*** option as shown in the image below.
***Power Query Editor -> File -> Remove Columns List -> Remove Columns***

<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_REMOVE_COLUMNS.jpg">
</p>






