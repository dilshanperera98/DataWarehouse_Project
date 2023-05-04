# DataWarehouse_Project

This is a project developed by using SQL Server Management Studio(SSMS), SQL Server Data Tools(SSDT) and Visual Studio. Here I created data warehouse using the data in a source database.
## Step 01 - Setting-up the Environment

#### Following tools are required to develop this project
• SQL Server Management Studio

• SQL Server Data Tools

• SQL Server 2016 or higher

• Microsoft Office (Excel/ Word)

#### Below database backups are required (Resources)

• RetailSourceDB.bak -> This database backup contains the source system data.

• CustomerAddress.txt -> This file contains all customer address information.


## Step 02 - Creating Databases and load data 

In here main data sources are relational tables in a source database and a flat file. As the first step, data needs to be extracted from the source systems (database and flat file) and loaded in the 'Staging' area, which is an intermediate storage between source systems and target, data warehouse. Data model/table structures of the 'Staging' database is very much closer the structure of the sources. Main difference is all the source tables/files are available in a single database server. Next step is to extract data from 'Staging'
database tables, transform data and load them into corresponding tables in dimensional model created in the data warehouse(ETL). This step will contain considerable transformation as the data warehouse tables are based on a dimensional model.



![Staging](https://user-images.githubusercontent.com/83137780/235994915-5ac3fa8f-a490-46f1-b729-7a98f6e4abfd.png)

![stagingSSDB](https://user-images.githubusercontent.com/83137780/235995009-38e6d068-af54-4ac2-a805-3616be9dc1eb.png)

![DW](https://user-images.githubusercontent.com/83137780/235995086-b42311f7-ef92-4404-9ec1-6513ee96dfb2.png)

![SCN](https://user-images.githubusercontent.com/83137780/235995131-953b3611-328a-463b-aab9-106659c54fea.png)

![RetailSSDB](https://user-images.githubusercontent.com/83137780/235995161-bd5e9666-c6cc-4227-9b36-3e6b9033ac65.png)
