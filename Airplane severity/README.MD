<p>	
 <h1>Predict the severity of an airplane accident</h1>	
</p>	

<h2>Problem statement</h2>	
Flying has been the go-to mode of travel for years now; it is time-saving, affordable, and extremely convenient. According to the FAA, 2,781,971 passengers fly every day in the US, as in June 2019. Passengers reckon that flying is very safe, considering strict inspections are conducted and security measures are taken to avoid and/or mitigate any mishappenings. However, there remain a few chances of unfortunate incidents.
<br></br>
Imagine you have been hired by a leading airline. You are required to build Machine Learning models to anticipate and classify the severity of any airplane accident based on past incidents. With this, all airlines, even the entire aviation industry, can predict the severity of airplane accidents caused due to various factors and, correspondingly, have a plan of action to minimize the risk associated with them.
<br></br>


https://www.hackerearth.com/problem/machine-learning/predict-the-energy-used-612632a9-3f496e7f/

<h2>Data description</h2>	

The dataset comprises 3 files: 

* Train.csv: [10000 x 12 excluding the headers] contains Training data
* Test.csv: [2500 x 11 excluding the headers] contains Test data
* sample_submission.csv: contains a sample of the format in which the Results.csv needs to be

Details of the train.csv file:

| Column Name  | Description |	
|------------|------------|
|Columns|	Description|
|Accident_ID|	unique id assigned to each row|
|Accident_Type_Code|	the type of accident (factor, not numeric)|
|Cabin_Temperature|	the last recorded temperature before the incident, measured in degrees fahrenheit|
|Turbulence_In_gforces|	the recorded/estimated turbulence experienced during the accident|
|Control_Metric|	an estimation of how much control the pilot had during the incident given the factors at play|
|Total_Safety_Complaints|	number of complaints from mechanics prior to the accident|
|Days_Since_Inspection|	how long the plane went without inspection before the incident|
|Safety_Score|	a measure of how safe the plane was deemed to be|
|Violations|	number of violations that the aircraft received during inspections|
|Severity	|a description (4 level factor) on the severity of the crash [Target]|


[Download Data](https://he-s3.s3.amazonaws.com/media/hackathon/airplane-accident-severity-hackerearth-machine-learning-challenge/how-severe-can-an-airplane-accident-be-03e7a3f1/3c055e822d5b11ea.zip?Signature=nMB6AzsKim2pYmwmVnroez2j2zs%3D&Expires=1613712171&AWSAccessKeyId=AKIA6I2ISGOYH7WWS3G5)

<h2>Evaluation Criteria</h2>

<img src="https://latex.codecogs.com/gif.latex?score&space;=&space;{100*&space;f1\_score(actual\_values,predicted\_values,average&space;=&space;'weighted')}" title="score = {100* f1\_score(actual\_values,predicted\_values,average = 'weighted')}" />

