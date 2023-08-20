# Hardware_company_sales_Analysis---SQL-to-PowerBI

# Problem Statement:
- AtliQ Hardware is a company which supplies computer hardware peripherals to many of the clients. They have this client called Surge stores, Nomad Stores, Excel Stores, Electricalsara Stores across India and they supply all these equipment to them .
  
-  Now AtliQ hardware has a head office in Delhi and other regional offices throughout India. 
Now, Bhavan Patel is a sales director for this company and he is facing a lot of challenges. One of the challenges would be about the market growth, and issues in terms of tracking the sales in this dynamically growing market. Another would be issues about the insights of his business. 

- He has this Regional Managers for North India, South India, and Central India. Whenever he gets insights about these three regions, he would call these people on the phone.  Then these regional managers will give him some insights about what was the sales last quarter and we going to grow by this much in the next quarter. 
The problem is the that, the conversation which are happening are just verbal.  Based from the statement of the owner, there are this habit that all the mangers try to paint a rosy picture and try to sugar coat some things. They don’t want to look bad. When Bhavin Patel ask for an Insights , they will give him a lot of excel files like 69 files. 

### CEO request
- Find what are the weakest areas that we need to focus.
- He is interested in getting a simple understandable digestible insight.
- He wants to see a dashboard where he can just open his chart and how the numbers trending.
- He wants to set daily email daily reminders.  At the end of the month, he wants PowerBi will send him an email saying that this is how the business looks in terms of revenue, customers etc. 

# Project Planning
- Using AIMS GRID and Data Discovery
![atliq](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/a14a714e-7bcf-412d-a696-73a501dc0ac5)


## NOTES:
- Falcons (Software Engineers) owns the management system that  AtliQ Hardware used. He has his sales use a management system that keeps track of all the sales number.  
Whenever they sell any computer or any products in any local region, it stores the data in Falcon’s DBMS 

![Screenshot 2023-08-19 215315](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/156285f9-031b-4911-ad32-24dcb2ac969f)


# Data Cleaning
-	Instead of doing data cleaning in SQL. This time data I  will be doing data analysis, data cleaning and data transformation through PowerBI.


### Under Markets table
- Two data ha no zone
  
![d1](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/42bffdae-530c-4179-9764-8a407dba5a26)

### Under the transactions
- Negative sales amount and zero amount can be recovered . Thus, I will  uncheck those to filter out my unnecessary data.

![d2](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/957bc5b9-e94f-429e-a40d-f30407aa8994)

![d3](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/7880d8f2-4252-4bda-bf54-639fbc7e0d5b)

- Some data has USD currency as well. Thus, I will be replacing it with USD. Right click the value and choose replace.
- Or use a formula “= Table.ReplaceValue(#"Filtered Rows","USD","INR",Replacer.ReplaceText,{"currency"}) “

  ![d4](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/29f04ac5-f024-4b81-aedb-36a5d012067f)

-	There are also duplicates detected via SQL. Using PowerBI, I removed all the duplicates, blank rows, and errors just to make sure that the data is clean. I applied it in all tables just to make sure as well. see images below on how I did it.

![d5](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/da065d7d-2f88-473c-ac91-306213d14f5d)

![d6](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/38ce73de-53bc-48a1-ac3a-ea354fca7f2b)

- I also have to rename some of the table columns because the data were manually imported as all csv and not through connecting MySQL database. This will just allow me to easily distinguish things up during data selection during my dashboard design.

  ![d7](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/f9ad59b1-7108-4a8d-94e5-b3dc2c415fd7)

# Dashboard Troubleshooting

####	Removing Blank Year in the slicer
-	The ‘blank’ year keeps appearing. I have tried looking in transform data section but it isn’t there. There are no data that says blank either.
  
-	So the only way to do it that I found is to filter it in the FILTERS SECTION in the report view where I am doing my dashboard. Then select  “IS NOT BLANK”

 ![d8](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/2d346add-594f-419a-bba5-7f2d93f40f09)


#### Format changing for the  Year slicer
-	Select data view. Then select column tools then change the format of the date into  (mm- yy ) for Jan 2018.
-	The data is from yyyy-mm-dd  transformed into mm-yy
  
-	1. First, select DATA View on the left side corner of the PowerBI
-	2.Second, choose the data table where you want to change the format

![d9](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/220549e3-f4e4-49ab-8d09-202ab4c27486)

- 3. Third, choose the column to be changed. Under the column tools, select 

![d10](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/594a508f-980b-46ba-a471-e4547e7fb653)




![giphy (1)](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/da4e6110-f0ca-4591-9ff8-1c344c79b1dc)









![AltiQ Financial Sales Analysis image](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/805823ad-6efd-49ec-afde-6a6d7be4063c)
