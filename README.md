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











![AltiQ Financial Sales Analysis image](https://github.com/lois4801/Hardware_company_sales_Analysis---SQL-to-PowerBI/assets/96842662/805823ad-6efd-49ec-afde-6a6d7be4063c)
