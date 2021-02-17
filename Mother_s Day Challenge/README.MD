<p>	
 <h1>Mother's Day Challenge</h1>	
</p>	

![Mother's Day Challenge](https://media-fastly.hackerearth.com/media/hackathon/hackerearth-machine-learning-challenge-mothers-day/images/09353cce9a-Mothers_Day_Cover.png)	

<h2>Problem statement</h2>	
While every day should be Mothers' Day [’cuz they rock], we are all guilty of taking to social media to post mushy messages or images on the second Sunday of May for our mothers. However, the Human Resources team of your organization wishes to celebrate and honor all moms currently employed at the company with a special monthly event. For one of such events, they have reached out to your team to curate and categorize Mothers’ Day-related tweets from across the globe.
<br><br>
As a Machine Learning Engineer, your task is to build a sophisticated sentiment analysis-based NLP model that can classify sentiments of tweets into positive, negative, and neutral.	
<br/>


https://www.hackerearth.com/challenges/competitive/hackerearth-machine-learning-challenge-mothers-day/

<h2>Data description</h2>	

The dataset consists of various parameters such as text and language of a tweet, the number of times it was retweeted, and the Twitter handle of the author.

This data set consists of six columns:	


| Column Name  | Description |	
| ------------- | ------------- |	
| id  | ID of tweet  |	
| original_text  | Text of tweet  |	
| lang  | Language of tweet  |	
| retweet_count  | Number of times retweeted  |	
| original_author  | Twitter handle of Author  |	
| sentiment_class	| Sentiment of Tweet (Target)| 

<p>The data folder consists of two .csv files. The details are as follows:</p>

* train.csv: 3235 x 6
* test.csv: 1387 x 5

<h2>Evaluation Criteria</h2>
![equation](https://latex.codecogs.com/gif.latex?score%20%3D%20%7B100*%20f1%5C_score%28actual%5C_values%2Cpredicted%5C_values%2Caverage%20%3D%20%27weighted%27%29%7D)

