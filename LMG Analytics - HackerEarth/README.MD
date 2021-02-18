<p>	
 <h1>LMG Analytics & Data Science Hiring Challenge</h1>	
</p>	

![LMG Analytics & Data Science Hiring Challenge](https://media-fastly.hackerearth.com/media/hackathon/LMG-analytics-data-science-hiring-challenge/images/e34a976ce0-Landmark_Group_HE_Cover-01.jpg)	

<h2>Problem statement</h2>	
Max is a fashion brand within Landmark Group and has launched certain new stores in the year 2018. The objective is to determine whether an existing customer of Max UAE will shop in each of the new stores.
<br></br>

https://assessment.hackerearth.com/challenges/hiring/LMG-analytics-data-science-hiring-challenge/machine-learning/max-customer-classification-to-shop-in-a-new-store/

<h2>Data description</h2>	

* Customer_Demographics: Customer demographics details for 100k customers •
* Customer_Transaction: Customer-Store-Week level transaction details for the last two years
* Store_Master: Store attribute details
* Test_Set: Submission file at Customer- New Store prediction level. Use this to create an additional column of Prediction tagging each customer-store into a 1 or a 0 for the submission file.

[Download Data](https://he-s3.s3.amazonaws.com/media/hackathon/Landmark-Group-Data-Scientist-Hiring-Challenge/max-customer-classification-to-shop-in-a-new-store/20ba1792-d-Data.zip)

<h2>Evaluation Criteria</h2>
F1 – Score at Customer Store level in the Test_Set for 1’s (Customers who buy in new stores)

<h2>Data Pre-Processing & Feature Engineering</h2>

1. Merging Customer_Transaction,Customer_Demographics,Store_Master data files
2. Imputed missing values in columns Geo_Field,Birth_date,First_txn_dt,Last_accr_txn_dt,Last_rdm_txn_dt
3. Converted string to date for columns First_txn_dt,Last_accr_txn_dt,Last_rdm_txn_dt,Store_Launch_Date,Birth_date
4. Created feature 'age' using column Birth_date
5. Extracted Week,year,date,month,season,day of week,day of year from date columns
6. Label encoded columns Geo_Field,Store_Name,Language,Nationality,Income_Range,Job_Type,Marital_Status,Gender,State,Language,Loyalty_Status,Region,Store_Name,Mall_Name
7. Splitted train data into X_train,y_train,X_test,y_test for training and validating the model

<h2>Model Building</h2>

1. Applied Following Models:
   1. Logistic Regression
   2. Random Forest
   3. Light Gradient Boosting Model
   4. KNN Classifier
   5. Decision Tree Classifier
   6. MLP Classifier
2. Applied grid search for hyper parameter tuning

<h2>Results</h2>

Secured rank of 88 rank in private leaderboard.

