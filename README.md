# NBA Rookie Analysis
This projeject attempts to leverage Machine Learning in python to create effective predictions for the next batch of NBA Rookies.
## 2019 College Clustering
The first file posted on this project gives a very top down view of the college stats of the players entering this years draft from college. Player data is visualized with a correlation matrix and cluster analysis to better understand the statistical distribution of players in this draft, and to look for certain similarities. The correlation matrix shows how strongly similar two varibles are just within the world of college stats. From there, the variables were decomposed, and three different methods of clusterings were employed. These three clustering methods were K-Means,Agglomerative, and Affinity Propagation, and they all all helped with visualizing similarities and overarching patterns.
## 	2019 NBA Prospect Scraper
This file documents the methodology and the source used for creating the 2019DraftClass.csv
## College+Rookie Data Cleaning
This file documents the methodology and the source used for creating the CollegeRookieStatLog.csv and the CollegeRookieStatLog2.csv
## Full College Clustering
Similar to the 2019 College Clustering, this file attempts to look at the college stats of all incoming rookies in the last 20 years. A correlation matrix was constructed to analyze basic feature similarities, and clustering algorithms were implemented to assess player similarities. Within the main objective of this project, Rookie Stats predictions, one main point of interest lied on what stats Zion Williamson would put up, given all the media commotion around him at the time of this project. One method of approaching this problem using clusters was to simply take the average of all the stats of the players in the same cluster as him. With that methodology, Zion Williamson is expected to put up 14.16 Points, 8.54 Rebounds, 3.38 Assists, 0.96 Steals, and 0.8 Blocks in his Rookie season.
## Rookie Predictions


*For this project, I had to webcrawl and webscrape data because there were no spreadsheets online that was extensive enough and structured to my liking. All the datasets I created for this project are now also available on Kaggle. (https://www.kaggle.com/siddhesvark/compiled-ncaa-basketball-data)
