## VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION
### Contents
1. Title
2. Tools Used
3. Description of Dataset
4. Importing Data & Combining Multiple CSV files
5. Filtering and Removing Duplicates & Unnecessary Columns
6. Data Transformation
8. Error Handling and Data Merging
9. Loading Cleaned Data into Excel/PowerBI for further analysis
----
### Tools Used
Microsoft Power Query Editor through MS-Excel/PowerBI

### Description of Dataset
The vehicle sales data has been collected from the <b>Regional Transport Authority Vehicle Online Sales Data</b> through a website https://data.telangana.gov.in/. The data between January 2023 to January 2024 were collected for performing data analysis and visualization using Business Intelligence Tool. The Excel files from January 2023 to January 2024 were combined using Microsoft Power Query Editor. The vehicle sales data consists of record_number, sl_no, modelDesc, fuel, color, vehicleClass, 
makeYear, seatCapacity, insuranceValidity, secondVehicle, tempRegistration, category, makerName, officecd, fromDate and toDate.

### Importing Data & Combining Multiple CSV files

The various csv files containing sales data for vehicles were kept together in a folder, from January 2023 to August 2023. The vehicle sales folder was loaded using power query editor.<br>

From Power Query tab, choose <b>From File</b> option, select <b>From Folder</b> options then type the folder path or browse the relevant 
folder from the dialog box.<br>
***Power Query -> From File -> From Folder -> Type or paste folder path or browse folder location -> Click Ok*** <br>

From Diaglog box, the required option as ***Combine & Edit*** were selected as shown below.
<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_DATA_1_LOADING%20FILES.jpg">
</p>

After selecting ***Combine & Edit*** option, the dialog box appears as below:

<p align="center">
  <img  src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_DATA_2_COMBINE_FILES.jpg">
</p>

After pressing ok button, by default, the power query editor will automatically check and applies the correct data type for all the columns. This step is automatically recorded in the ***Applied Steps***. Sometimes, the given data type for the columns may not be correct. Then, data type can be changed by selecting the specific column and choosing the required data type from the ***Transform*** tab option.

***Power Query -> From Transform -> Data Type: Any list -> Select required data type***


### Removing Unnecessary Columns

The vehicle sales data consists of 16 columns such as record_number, sl_no, modelDesc, fuel, color, vehicleClass, 
makeYear, seatCapacity, insuranceValidity, secondVehicle, tempRegistrationNumber, category, makerName, officecd, fromDate and toDate. From the vehicle sales data, 8 unwanted columns as record_number, sl_no, makeYear, seatCapacity, insuranceValidity, secondVehicle, officecd and toDate were removed by selecting all the columns and choosing ***Remove Columns*** from home menu or right clicking mouse on the one of the selected column and choose ***Remove*** option as shown in the image below.

***Power Query Editor -> Home -> Remove Columns List -> Remove Columns***

<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_REMOVE_COLUMNS.jpg">
</p>

### Removing Duplicates 

The duplicates from the vehicle sales data were removed based on the tempRegistrationNumber, after selecting the column and choosing ***Remove Duplicates*** from Remove Rows list.

***Power Query Editor -> Home -> Remove Rows list -> Remove Duplicates***

<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_DATA_5_DUPLICATES.jpg">
</p>

### Filtering Columns

The power query filters were applied to the vehicle sales data, illustrated below, based on the non-transport category.

<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_FILTER_CATEGORY.jpg">
</p>

As shown below, the rows of vehicle sales data were filtered according to the type of vehicle, such as motorcars.

<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_FILTER_VEHICLE_CLASS.jpg">
</p>

### Data Transformation

***- Inserting new column*** <br>
The new column year were inserted based on fromdate by using ***Column From Examples*** from Add Column tab.

***Select column -> Add Column -> Column From Examples -> From Selection ->Select the checkbox for the required column(fromdate selected)***

***- Data Type Changing or Applying***<br>
The data type for the particular column can be applied or changed by selecting the specific column and choosing the required data type from the ***Transform*** tab option or simply by selecting the icon on the left side of the column heading.

***Power Query -> From Transform -> Data Type: Any list -> Select required data type***

<p align="center">
  <img src="https://github.com/Tungana-Bhavya/VEHICLE_SALES_DATA_ANALYSIS_AND_VISUALIZATION/blob/main/IMAGES/VEHICLE_SALES_DATA_TYPE.jpg">
</p>

***- Removing and Reordering Columns***<br>
The column named ***fromDate*** from vehicle sales data were removed and also data columns were reordered as year, tempRegistrationNumber, category, fuel, vehicleClass, modelDescription, makerName and color.

