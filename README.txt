MAster course: Social Media Analytics: 
name fo project “sentiment indicator for cryptocurrency ticker apps”
*Designed and developed a functionality able to deliver sentiment analysis(over time and updated word cloud) over a chosen cryptocurrency/stock
*The final prototype surges after the definition of target personas, thinking hat analysis and customer journey mapping, the data analysis workflows and all of them are in the pdf report.

#CODE:
Crypto tweets collector:
1-Connecting and login through the twitter API, 
2-Using the Tweepy package to define the streaming tweets collector.
 - connecting to local Mysql database , using database package, to store all collected tweets
3-run the listener for several days. 

Tweets processing:
1- import all libraries, packagesused : pandas, textblop, nlkt,wordcloud...
2- export from database collected tweets and load them o a dataframe
3- clean Nan values
4- define set of stopwords and emoticons
5- define clean tweets function (punctiation, url links.. etc...)
6- apply sentiment analysis.  obtaining wordlcloud and aggregated timeseries of polarity scores of the twwets by hour,