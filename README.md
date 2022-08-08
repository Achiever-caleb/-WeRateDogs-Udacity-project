# Analysis for TMDb movie data set
## By Caleb Okon

### Introduction and Summary of Analysis

 
In this Project, i worked with three datasets

I was asked to download the first data manually and upload it to my workspace, then download the second one programmatically using Request function and gather additional datas from Twitter API using tweepy. but at the time of sending this report, twitter is yet to approve my developers account so i went with the other option which is using an altenate file provided by UDACITY.

During the wrangling process, i found 10 quality issues and 3 tidiness issues and i cleaned them up.In this Project, i worked with three datasets

I was asked to download the first data manually and upload it to my workspace, then download the second one programmatically using Request function and gather additional datas from Twitter API using tweepy. but at the time of sending this report, twitter is yet to approve my developers account so i went with the other option which is using an altenate file provided by UDACITY.

During the wrangling process, i found 10 quality issues and 3 tidiness issues and i cleaned them up.

#### key steps
I used the udacity project work space for my work and i took the following steps to complete my work

Gathering data - i gathered the data from multiple sources. i was asked to download the first data manually and upload it to my workspace, then download the second one programmatically using Request function and gather additional datas from Twitter API using tweepy. but at the time of sending this report, twitter is yet to approve my developers account so i went with the other option which is using an altenate file provided by UDACITY.

Assessing data - After gathering all my data successfully, i proceeded to to assessing it in order to check for errors that need to be fixed. i assessed it using two method;

Visually: I viewed the 3 data set individually to spot out peculiar issues associated with it
Programmatically: I also used various fuctions like .shape(), .duplicated(), .value_counts(), .info() to check the datas.
Cleaning data - I used the following format to clean the data:

Issues: this is where i state the particular problem i want to clean
Define: i stated how i intended to solve the problem here
Code: i insert my code here
test: here i put to test my code.

for the first dataframe named 'df', i made the following cleaning effort

eliminated the in_reply_to_status_id,in_reply_to_user_id, expanded_urls, retweeted_status_id, retweeted_status_user_id and retweeted_status_timestamp columns, because they contain mostly missing values and also, i will not be needing them for my analysis.

I also changed Tweet_id column which initially displays as INT64 and timestamp which initially displays as object, to Object and datetime datatype respectivel.

i replaced those data where the dog names in the Name column are not names of dogswith "None"

For the second dataset with name 'df2'

I changed Tweet_id to string and I changed the output of columns p1, p2 and p3, which had inconsistent format prieviously all lower case.

for the third dataset

I changed the Tweet_id column displays INT64 as datatype instead of Object

i also tidied them up and finally merged them into one dataset.

Storing Data: finally i stored the dataas a csv file named twitter_Archive_master.csv


#### Key Insights
1.The minimum favorite_count is o, the mean is 9005.25 and the maximum is 132,810

2. The minimum retweet_count is o, the mean is 3520.19 and the maximum is 79,515

3. more than 32% of the dogs in the data set have none in their name

4.columns in the dataset are 'tweet_id', 'timestamp', 'source', 'text', 'rating_numerator', 'rating_denominator', 'name', 'dog_stages', 'jpg_url', 'img_num', 'p1', 'p1_conf', 'p1_dog', 'p2', 'p2_conf', 'p2_dog', 'p3', 'p3_conf', 'p3_dog', 'id', 'retweet_count', 'favorite_count'.
5. the Top 5 are pupper, doggo, puppo, doggopupper and floofer. 