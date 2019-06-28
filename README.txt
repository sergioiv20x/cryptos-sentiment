 Social Media Analytics project: lets call it a “Sentiment indicator for cryptocurrency ticker apps”
*Designed and developed a functionality able to deliver sentiment analysis(over time and updated word cloud) over a chosen cryptocurrency/(it can also be applied to stocks)
*The final prototype surges after the definition of target personas, thinking hat analysis and customer journey mapping, the data analysis workflows and all of them are in the FINAL PDF REPORT better detailed.

#CODE: (is better commented on the ipynb files, this is just generaly what i did)
Crypto tweets collector:
1-Connecting and login through the official twitter API
2-Using the TWEEPY package to define the streaming tweets collector/listener.  (DATA GATHERING)
 - connecting to local Mysql database , using DATABASE package, to store all collected tweets (DATA STORING)
3-run the listener for several days. 

Tweets processing:
1- import all libraries.  packagesused : PANDAS, textblop, nlkt, wordcloud...
2- export from database collected tweets and load them o a dataframe (EXTRACT DATA)
3- clean Nan values (DATA CLEANING) and define set of stopwords and emoticons (DATA CLEANING & Profiling for Natural language processor)
5- define "clean tweets" function (punctiation, url links.. etc...)   (more cleaning before processing and scoring the tweets)
6- apply sentiment analysis.  obtaining Wordlcloud and an  aggregated timeseries with the polarity scores of the tweets hourly.

