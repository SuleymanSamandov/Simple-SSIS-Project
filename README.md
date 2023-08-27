# Project design
![Screenshot 2023-08-26 193655](https://github.com/SuleymanSamandov/Simple-SSIS-Project/assets/98223056/31385903-55bc-48ad-92ba-bef72eec2b9d)

It can be used to fetch data from the project data source and write it to target systems. With the write generated against duplication of data. 
And when there is any update in the data, it is recorded in the Dump table. Then the target table is updated.

![Screenshot 2023-08-26 193631](https://github.com/SuleymanSamandov/Simple-SSIS-Project/assets/98223056/71590393-6980-455e-8ac6-f852092516b2)

Truncate Table Cleans the Dump table to avoid duplication after data is retrieved from the SQL Task Dump table and the target table is updated.

Max Date Filter SQL Task is used to get latest records.

The latest Execute SQL Task is used to update the target table.
