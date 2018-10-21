# Trending-Movie-Data-Analysis-and-Database-Design

Intro
Our database project is in the field of movie and the specific perspective is 1000 high rated movies in the last ten years.

We use movie names as keywords to scrape tweets from social network like Twitter in order to get information like audience information (user who post relative posts about specific movie) and then this data can be used to analyze audience distribution condition, audience’s influence, etc. Also, the tag information will help us to define the movie’s influence and different views towards it. 
Part 1-Source Data Cleaning
Initially the dataset is in one csv tables, therefore we divide them into 4 csv tables according to our E-R diagrams.

Then we import those 4 csv tables into Jupyter Notebooks and conduct basic data cleaning through remove duplicated values, empty values or multiple values in a single column.
Part 2-Scrape from Twitter
For now, we will be using the movie main csv table we created as keywords to scrape data from Twitter. The reason why we use Twitter is that:
    1. There are many tutorials you can learn
    2. The API is very friendly and we can get the information we need with ease.
3. Documentation is clear too.

The major part here is to ran the scraping code which really takes time. although twitter is a very good source for data scraping, it also has its own disadvantage. For one, it has limitation on the volume of data you can get at the same time. Therefore, we registered 10 usernames, and get those data in 10 times, each time we scrape data about 100 movies. 

Then we will copy and paste this data into Excel and conduct the initial data cleaning. Then we will use python to check the duplicate & null values.

After these steps, we now have a cleaned Twitter user and twitter tag tables.
Part 3 – Scrape from YouTube
YouTube is another data source we choose.
We choose YouTube instead of Instagram / Facebook because it is easy to collect a lot of tags at the same time, while Instagram & Facebook now has strict rules to limit your scraping.

We again use several accounts to conduct the scraping at the same time. Then we will copy and paste this data into Excel and conduct the initial data cleaning. Then we will use python to check the duplicate & null values.
Part 4 – Answer Question
We will use our database to answer the 12 given questions.

Part 5 – Synonym 
We will use NLTK wordnet to do the synonym analysis. We will read the existing synsets that have same meaning with the tag we input and then store that information.

Major endeavor is to clean the data which always repeat themselves. And we will import those data into our database.
Part 6 - Sentiment
Sentiment Analysis here is to find the categories of tags. We will be using WordNet hypernyms function to conduct it.

Hypernyms means a bigger concept here. And in a way can show the meaning of this tag.

The following example here show that the hypernyms of "woman" will be adult or female, which to a certain extent show woman’s sentiment.
 
From operation level, we find and print all the existing hypernyms of tags in the form of csv and import the csv table to further data cleaning.

