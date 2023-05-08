# taliban-twitter-network
## Social network analysis for biggest taliban accounts on twitter

This is the first part of a project to analyze the social network of Taliban members' accounts on Twitter and their tweets. 

In this part, the data is being scraped from Twitter using the Twitter API V2 and Tweepy library. 

A list of known Taliban liders' IDs (those were not confirmed by Twitter) and their followers' IDs with more than 1000 followers was created. The snowball sampling method was applied, so other significant IDs and their followers have been added to the list.

Getting Followers notebook collects username, user-id, name (screen name), created at, followers count, following count, tweet counts and the list of followers that have more than 1000 followers for a given ID. Example of results: AnasHaqqani - Data.csv, Bilal Karimi - Karimi.csv, Naeem - Naeem.csv

Test set - mutual following notebook scrapes data of mutual following between the chosen IDs and stores results in results1.csv (results 2.csv is the same matrix with integers instead of strings, needed for creating graphs). 

Scraping Tweets notebooks scrapes tweets of a given ID for a specific time period, in this case period of Taliban offensive.

Taliban Twitter Network Test - testing a few network metrics using the results1.csv and followers-following-all-users.xlxs.
