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
<img src="https://latex.codecogs.com/gif.latex?score&space;=&space;{100*&space;f1\_score(actual\_values,predicted\_values,average&space;=&space;'weighted')}" title="score = {100* f1\_score(actual\_values,predicted\_values,average = 'weighted')}" />

<h2>Data Pre-Processing & Feature Engineering</h2>
1 Target Variable has -1,0,1 for indicating negative,neutral,positive tweets. Updated those to 0,1,2 because xgb.cv giving error as label should be in [0.num_class]
2 Used HTML Parser to convert all named and numeric character references (e.g. &gt;, &#62;, &#x3e;) in the string s to the corresponding Unicode characters.
3. Used regex to replace all URL's like twitter.com,instagram.com from the tweets
4. Extracted only words from the tweets
5. Converted entire text to lower case
6. Created Apostrophe Dictionary to change the words having Apostrophe in the tweets
7. Updated words in tweets which has short hand words
8. Created and used to emoji dictionary to update all emoji's in tweets
9. Counted all the hashtags and added as feature to the data
10. 
11. 
              1. A nested numbered list
              2. Which is numbered
          2. Which is numbered

