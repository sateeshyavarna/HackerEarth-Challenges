<p>	
 <h1> Predict the damage to a building </h1>	
</p>	

<h2>Problem statement</h2>	
Determining the degree of damage that is done to buildings post an earthquake can help identify safe and unsafe buildings, thus avoiding death and injuries resulting from aftershocks.  Leveraging the power of machine learning is one viable option that can potentially prevent massive loss of lives while simultaneously making rescue efforts easy and efficient.
<br></br>
In this challenge we provide you with the before and after details of nearly one million buildings after an earthquake. The damage to a building is categorized in five grades. Each grade depicts the extent of damage done to a building post an earthquake.
<br></br>
Given building details, your task is to build a model that can predict the extent of damage that has been done to a building after an earthquake.	
<br/>


https://www.hackerearth.com/problem/machine-learning/predict-the-energy-used-612632a9-3f496e7f/

<h2>Data description</h2>	

You’re give four files: train.csv, test.csv, Building_Ownership_Use.csv and Building_Structure.csv.

Details of the train.csv file:

| Column Name  | Description |	
|------------|------------|
|area_assesed|Indicates the nature of the damage assessment in terms of the areas of the building that were assessed|
|building_id|A unique ID that identifies every individual building|
|damage_grade|Damage grade assigned to the building after assessment (Target Variable)|
|district_id|District where the building is located|
|has_geotechnical_risk|Indicates if building has geotechnical risks|
|has_geotechnical_risk_fault_crack|Indicates if building has geotechnical risks related to fault cracking|
|has_geotechnical_risk_flood|Indicates if building has geotechnical risks related to flood|
|has_geotechnical_risk_land_settlement|Indicates if building has geotechnical risks related to land settlement|
|has_geotechnical_risk_landslide|Indicates if building has geotechnical risks related to landslide|
|has_geotechnical_risk_liquefaction|Indicates if building has geotechnical risks related to liquefaction|
|has_geotechnical_risk_other|Indicates if building has any other  geotechnical risks|
|has_geotechnical_risk_rock_fall|Indicates if building has geotechnical risks related to rock fall|
|has_repair_started|Indicates if the repair work had started|
|vdcmun_id|Municipality where the building is located|

[Download Data](https://he-s3.s3.amazonaws.com/media/hackathon/machine-learning-challenge-6-1/predict-the-energy-used-612632a9-3f496e7f/a490e594-6-Dataset.zip)

<h2>Evaluation Criteria</h2>

Evaluation is based on F1 Score with 'weighted' average.

<h2>Data Pre-Processing & Feature Engineering</h2>

1. Imputed Missing values in columns(has_repair_started,count_families)
2. Label Encoded for the columns(land_surface_condition,roof_type,damage_grade)
3. Removed highly correlated(correlation > 0.7) columns(has_geotechnical_risk_landslide ,has_secondary_use_agriculture ,height_ft_post_eq ,height_ft_pre_eq ,vdcmun_id ,ward_id_x ,condition_post_eq_Damaged-Repaired and used,condition_post_eq_Damaged-Rubble clear 
4. Splitted the train data into X_train,y_train,X_test,y_test for training and validating the model

<h2>Model Building</h2>

1. Used XGBoost,Random Forest model to build the predictions 
2. Applied grid search for hyper parameter tuning


