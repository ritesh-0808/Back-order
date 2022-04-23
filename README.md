# Back-order

Problem Statement-

    To build a model which will be able to predict whether an order for a given product can go on backorder or not. 
    A backorder is the order which could not be fulfilled by the company. Due to high demand of a product, the company was not able to keep up with the delivery of the order.

 

 

![image](https://user-images.githubusercontent.com/76938173/162598730-966a4242-1224-4cfb-b823-18d6fa4d578e.png)

![image](https://user-images.githubusercontent.com/76938173/162598803-23bc1aaa-1852-4497-bf29-24904095eca3.png)

![image](https://user-images.githubusercontent.com/76938173/162598863-df55fa54-e5cf-41be-af5a-af5c610064f5.png)






Project Architecture 

![image](https://user-images.githubusercontent.com/76938173/162401484-9ec75c9c-7d0f-4dfc-9048-313417f4e4f7.png)


Data Description-

     The client will send data in multiple sets of files in batches at a given location. Data will contain 24 columns: 
     
      sku – 		 	Random ID for the product
      national_inv –   	Current inventory level for the part
      lead_time – 	 	Transit time for product (if available)
      in_transit_qty – 	Amount of product in transit from source
      forecast_3_month – 	Forecast sales for the next 3 months
      forecast_6_month – 	Forecast sales for the next 6 months
      forecast_9_month – 	Forecast sales for the next 9 months
      sales_1_month – 	Sales quantity for the prior 1 month time period
      sales_3_month – 	Sales quantity for the prior 3 month time period
      sales_6_month – 	Sales quantity for the prior 6 month time period
      sales_9_month – 	Sales quantity for the prior 9 month time period
      min_bank – 		Minimum recommend amount to stock
      potential_issue – 	Source issue for part identified
      pieces_past_due – 	Parts overdue from source
      perf_6_month_avg – 	Source performance for prior 6 month period
      perf_12_month_avg – 	Source performance for prior 12 month period
      local_bo_qty – 		Amount of stock orders overdue
      deck_risk – 		Part risk flag
      oe_constraint – 	Part risk flag
      ppap_risk – 		Part risk flag
      stop_auto_buy – 	Part risk flag
      rev_stop – 		Part risk flag
      went_on_backorder – 	Product actually went on backorder. This is the target value.

      Apart from training files, we also require a "schema" file from the client, which contains all the relevant information about the training files such as:
      Name of the files, Length of Date value in FileName, Length of Time value in FileName, Number of Columns, Name of the Columns, and their datatype.
 
 
![2022-04-23 (2)](https://user-images.githubusercontent.com/76938173/164883407-bb202bd3-e72f-429a-9171-6e4816dd7b46.png)

Training logs

![2022-04-23 (3)](https://user-images.githubusercontent.com/76938173/164883413-ad1a20ad-a7b8-4f57-9981-315399baaae4.png)

![2022-04-23 (4)](https://user-images.githubusercontent.com/76938173/164883427-7e3e376f-4287-4640-87d7-ea056ff23b1a.png)

![2022-04-23 (5)](https://user-images.githubusercontent.com/76938173/164883433-387dabcb-4bb1-442d-b314-d100b52a8cfc.png)

![2022-04-23 (6)](https://user-images.githubusercontent.com/76938173/164883440-ccab29c6-861c-4ce0-bf95-53542e8c0d46.png)

![2022-04-23 (7)](https://user-images.githubusercontent.com/76938173/164883471-6e4e3506-e817-4ab9-88a9-3e5850f44a4f.png)

![2022-04-23 (8)](https://user-images.githubusercontent.com/76938173/164883481-def1057d-e2c0-4218-af5c-9ce7e0d6327b.png)

![2022-04-23 (9)](https://user-images.githubusercontent.com/76938173/164883487-0808aa3f-9d61-4025-a12e-ed2f2d74f9de.png)

![2022-04-23 (10)](https://user-images.githubusercontent.com/76938173/164883502-44a1d237-a21a-4e5e-9edd-95d74933faad.png)

![2022-04-23 (11)](https://user-images.githubusercontent.com/76938173/164883509-d8dd4e1a-1e4f-4788-99f3-e74826b7dffe.png)

![2022-04-23 (12)](https://user-images.githubusercontent.com/76938173/164883525-c33102da-b2e7-4641-9118-50490259c731.png)

![2022-04-23 (13)](https://user-images.githubusercontent.com/76938173/164883531-06ed35ab-603e-4992-8951-3a5a6a525d52.png)

![2022-04-23 (14)](https://user-images.githubusercontent.com/76938173/164883544-e00b9178-cbcc-4347-a218-61a73de59219.png)

![2022-04-23 (14)](https://user-images.githubusercontent.com/76938173/164883555-e6cdffeb-b6e5-4ea9-842a-82f12c132511.png)



https://user-images.githubusercontent.com/76938173/164885810-8a801a5b-2fa3-4ec1-bca2-64eb8f2240c3.mp4


 
![2022-04-23 (15)](https://user-images.githubusercontent.com/76938173/164883564-b81c7341-d7bd-49ae-988d-a5fdc0bd9c96.png)

![2022-04-23 (16)](https://user-images.githubusercontent.com/76938173/164883570-0e50907a-40d2-4dca-a0c7-e365465248e1.png)


Exploratory Data Analysis



https://user-images.githubusercontent.com/76938173/164885846-1d21c5cf-f710-41ae-8db2-27bdbba348fd.mp4


Prediction  Logs


![2022-04-23 (17)](https://user-images.githubusercontent.com/76938173/164885914-3ff58edd-5b23-46d7-8943-4d80d24901f5.png)

![2022-04-23 (18)](https://user-images.githubusercontent.com/76938173/164885934-64a5da2a-aac0-4cfc-8c25-2b27b993065f.png)
![2022-04-23 (19)](https://user-images.githubusercontent.com/76938173/164885949-67dd2e19-2475-433a-959c-bc25b9273400.png)

![2022-04-23 (20)](https://user-images.githubusercontent.com/76938173/164885958-a9fe4f76-6d92-4ebe-9b55-59665a7014ed.png)
 
 ![2022-04-23 (21)](https://user-images.githubusercontent.com/76938173/164885996-e3d96066-5cfc-4aa4-bc39-b31ceb55d119.png)

 ![2022-04-23 (22)](https://user-images.githubusercontent.com/76938173/164886003-245a1858-cb5e-4b19-8de9-f62beab8fffd.png)

 ![2022-04-23 (23)](https://user-images.githubusercontent.com/76938173/164886009-9e99dd99-4bcc-47ee-a616-538d847a136c.png)

 ![2022-04-23 (24)](https://user-images.githubusercontent.com/76938173/164886016-fca93540-2cdb-459a-bbdf-b9b92a0e68da.png)

 ![2022-04-23 (25)](https://user-images.githubusercontent.com/76938173/164886025-6a7a83bc-3032-4b0a-876b-9a2787f84fdb.png)

 ![2022-04-23 (26)](https://user-images.githubusercontent.com/76938173/164886054-911076c9-15f9-430c-a480-a91cb5f68e91.png)

 
 
 
 ![2022-04-23 (27)](https://user-images.githubusercontent.com/76938173/164886062-ccaefd56-337f-49c0-a838-22f98743b86d.png)

 ![2022-04-23 (28)](https://user-images.githubusercontent.com/76938173/164886073-eb1b3548-ed41-49b6-a620-28ab2a25e171.png)

 
 
 
 
 

Data Validation -
   
   In this step, we perform different sets of validation on the given set of training files.  
   
     1. Name Validation- We validate the name of the files based on the given name in the schema file. We have created a regex pattern as per the name given in the schema file to use for validation. After validating the pattern in the name, we check for the length of date in the file name as well as the length of time in the file name. If all the values are as per requirement, we move such files to "Good_Data_Folder" else we move such files to "Bad_Data_Folder."

     2. Number of Columns - We validate the number of columns present in the files, and if it doesn't match with the value given in the schema file, then the file is moved to "Bad_Data_Folder."


     3.	Name of Columns - The name of the columns is validated and should be the same as given in the schema file. If not, then the file is moved to "Bad_Data_Folder".

     4. The datatype of columns - The datatype of columns is given in the schema file. This is validated when we insert the files into Database. If the datatype is wrong, then the file is moved to "Bad_Data_Folder".


     5. Null values in columns - If any of the columns in a file have all the values as NULL or missing, we discard such a file and move it to "Bad_Data_Folder".

Data Insertion in Database-

      1) Database Creation and connection - Create a database with the given name passed. If the database is already created, open the connection to the database. 
   
      2) Table creation in the database - Table with name - "Good_Data", is created in the database for inserting the files in the "Good_Data_Folder" based on given column names and datatype in the schema file. If the table is already present, then the new table is not created and new files are inserted in the already present table as we want training to be done on new as well as old training files.   
   
      3) Insertion of files in the table - All the files in the "Good_Data_Folder" are inserted in the above-created table. If any file has invalid data type in any of the columns, the file is not loaded in the table and is moved to "Bad_Data_Folder".


Model Training -

    1) Data Export from Db - The data in a stored database is exported as a CSV file to be used for model training.
    
    2) Data Preprocessing   
      a) Drop columns not useful for training the model. Such columns were selected while doing the EDA.
      b) Replace the invalid values with numpy “nan” so we can use imputer on such values.
      d) Check for null values in the columns. If present, impute the null values 
      e) Scale the training and test data separately 
      
    3) Clustering - KMeans algorithm is used to create clusters in the preprocessed data. The optimum number of clusters is selected by plotting the elbow plot, and for the dynamic selection of the number of clusters, we are using "KneeLocator" function. The idea behind clustering is to implement different algorithms
       To train data in different clusters. The Kmeans model is trained over preprocessed data and the model is saved for further use in prediction.
       
    4) Model Selection - After clusters are created, we find the best model for each cluster. We are using two algorithms, "Decision Tree Regressor" and "XGBoost regressor". For each cluster, both the algorithms are passed with the best parameters derived from GridSearch. We calculate the Rsquared scores for both models and select the model with the best score. Similarly, the model is selected for each cluster. All the models for every cluster are saved for use in prediction. 
 
Prediction Data Description-

     Client will send the data in multiple set of files in batches at a given location. Data will contain climate indicators in 10 columns.
     Apart from prediction files, we also require a "schema" file from client which contains all the relevant information about the training files such as:
     Name of the files, Length of Date value in FileName, Length of Time value in FileName, Number of Columns, Name of the Columns and their datatype.

 Data Validation-
      
      In this step, we perform different sets of validation on the given set of training files.  
      
       1) Name Validation- We validate the name of the files on the basis of given Name in the schema file. We have created a regex pattern as per the name given in schema file, to use for validation. After validating the pattern in the name, we check for length of date in the file name as well as length of time in the file name. If all the values are as per requirement, we move such files to "Good_Data_Folder" else we move such files to "Bad_Data_Folder". 
       
       2) Number of Columns - We validate the number of columns present in the files, if it doesn't match with the value given in the schema file then the file is moved to "Bad_Data_Folder". 
       
       3) Name of Columns - The name of the columns is validated and should be same as given in the schema file. If not, then the file is moved to "Bad_Data_Folder". 
       
       4) Datatype of columns - The datatype of columns is given in the schema file. This is validated when we insert the files into Database. If dataype is wrong then the file is moved to "Bad_Data_Folder". 
       
       5) Null values in columns - If any of the columns in a file has all the values as NULL or missing, we discard such file and move it to "Bad_Data_Folder".  


Data Insertion in Database -

       1) Database Creation and connection - Create database with the given name passed. If the database is already created, open the connection to the database. 
       
       2) Table creation in the database - Table with name - "Good_Data", is created in the database for inserting the files in the "Good_Data_Folder" on the basis of given column names and datatype in the schema file. If table is already present then new table is not created, and new files are inserted the already present table as we want training to be done on new as well old training files.  
       
       3) Insertion of files in the table - All the files in the "Good_Data_Folder" are inserted in the above-created table. If any file has invalid data type in any of the columns, the file is not loaded in the table and is moved to "Bad_Data_Folder".

Prediction -

     1) Data Export from Db - The data in the stored database is exported as a CSV file to be used for prediction.
     
     2) Data Preprocessing   
        a) Drop columns not useful for training the model. Such columns were selected while doing the EDA.
        b) Replace the invalid values with numpy “nan” so we can use imputer on such values.
        c) Check for null values in the columns. If present, impute the null values.
        d) Scale the training data.
        
     3) Clustering - KMeans model created during training is loaded, and clusters for the preprocessed prediction data is predicted.
     
     4) Prediction - Based on the cluster number, the respective model is loaded and is used to predict the data for that cluster.
     
     5) Once the prediction is made for all the clusters, the predictions along with the original names before label encoder are saved in a CSV file at a given location and the location is returned to the client.
 
 ![image](https://user-images.githubusercontent.com/76938173/164886301-0a2dcdeb-a8d8-4d19-936e-fb610a39321a.png)

