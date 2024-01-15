# How to create Google Cloud SQL Server instance and connect from SSMS, VSCode and Visual Studio 2022 Community Edition

See this video: https://www.youtube.com/watch?v=ELTI7eS1Kdk

## 1. Create Google Cloud SQL Server instance

We search for SQL in the components searching text box

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/79bf55c7-2e5f-442c-bb02-737c2f40fdf4)

We select SQL->Managed MySQL, PostgreSQL, SQL Server

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/69ce9231-9779-49fe-9d7d-a6372c306ea8)

We choose SQL Server option

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/3bf57378-9791-48f1-9256-7a7e62dfa75b)

We input the server name, database password and Development option

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/d5ecb9ae-ba5f-4db4-a56c-3ff1e189a6d1)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/a1cbb7a0-e788-4867-8797-ea44a4121dd9)

We select a Single zone and input the Region/location

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/2480cb8b-6b60-4e54-b1ee-4df132c83b68)

We select the CPU/Memory and storage capacity

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/0152843b-d15d-42ad-9e17-8f9d6cfe050c)

We select the Public IP in the Connection details

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/2b01ea0e-20ff-4726-b8ec-65fec05ac293)

We add my laptop local IP and we press the **Add a Network** button

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/798b44e2-d445-4529-9d4f-7d437d3617c4)

**IMPORTANT NOTE**: to get you local laptop IP navigate to the https://www.whatismyip.com/

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/05067c8b-37e4-4bb3-b8cf-88d9fe055467)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/987751e5-5631-4584-ab0a-b52bf42726c6)

We unselect the **Enable deletion protection** option

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/bae2d197-618d-48b6-a0b5-825a546a4ab8)

In **Featured Flag Setting** we select **Enable SQL Server Audit**

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/89571a0d-c2a4-476e-bec1-16d7b9358cc8)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/9b6ae0fc-8a52-45d5-b1e8-5f73845e86e9)

We create a new bucket for database logs

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/775d7368-277a-4eb1-a2fa-589519d5e9a2)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/3ac56b13-ee33-4c02-ad5b-6e9c696714e4)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/b15e6a6c-fe0e-429c-b381-5ad0acfec123)

We create a new folder inside the bucket

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/b11f8c10-5eda-4c6f-b5c6-32c7e7a51021)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/93ec0439-955a-478f-b8e0-14b1224992a5)

We select the folder inside the bucket

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/86d09063-2e03-4c43-8a11-afaec34e4ada)

We verify we select the folder

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/41715cbf-e548-4928-8c38-8c83e0eb1157)

Finally we press the **CREATE INSTANCE** button

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/3344a8ac-8397-4f32-bd6e-2c46af0b40af)

We verify we are creating a nw SQL Server instance

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/3fba46ef-3dfc-4975-8a31-632b5a326143)

We can see the new SQL Server instance in the list

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/52c79a80-2192-4fa7-8789-d5d1b0c99e12)

We can press ths **Column display options** button to add more fields info

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/0ad4cb7c-33f3-4272-b605-220bacf15d66)

The most important infor to copy for connecting to the database is the Public IP and the database user

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/c6a3dd11-c5b2-4df0-b377-aedba845617d)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/8e10ed5f-981f-4d3c-978a-150b100d434a)

## 2. Connect to Google Cloud SQL instance from SSMS

We run SSMS and we enter the SQL Server name and password

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/6c10be5b-a6f0-4fe4-ab45-257b72b62b2b)

We can create a new database

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/4a48196a-e80e-4b09-a03f-a80d5fc4a395)

## 3. Connect to Google Cloud SQL instance from VSCode

We VSCode and we press **SQL Server** button in the left hand side menu 

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/2f2b04a3-ae62-42bc-b591-aee6a40a024c)

We create a new connection

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/bc230512-04fe-41ec-b7db-c90800611b3d)

We input the Public IP in the server name

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/8cfcb0a6-1415-406b-a00c-1d36a40a1160)

We do not input any database name, we just press enter button

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/a7602b6a-e55c-48c4-9327-c9c12726b690)

We select SQL login option

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/548f474d-2f69-4649-9420-7fe52c947612)

We input the **sqlserver** user

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/2490d49c-7879-4dca-9e89-d78caae333ac)

We input the **database password**

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/64f2b6f6-b633-40f7-b6ee-656660307d1f)

We leave the default value for profile name

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/f74c48bc-c1fa-4193-aade-c127033de24d)

We also press **Enable Trust Server Certificate**

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/2d0b90ab-1de0-400c-8aa3-9bf104ce98d9)

We verify the SQL Server connection

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/67c42a06-0ab3-41c1-8d84-a7fb1d3773cd)

## 4. Connect to Google Cloud SQL instance from Visual Studio 2022 Community Edition

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/d1dbb1cf-5d4b-4578-abd1-389728e8d81c)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/dfe6dc07-a349-4efd-8afc-a16043f24cd6)

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/63944228-68ec-4e16-80a2-1f22e062815a)

We add a new SQL Server connection

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/385892da-aa93-4395-a80c-0fd364a1f652)

We input the connection data

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/812d5ba4-ac5a-45d8-9a34-56016685aedf)

We verify the new SQL Server connection

![image](https://github.com/luiscoco/GoogleCloud_Sample12-Create-a-SQL-Server-instance/assets/32194879/038f72a0-57c6-405f-b936-e06aaa1bf4a7)


