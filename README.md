# NBA Rookie Analysis

![image](https://cdn.vox-cdn.com/thumbor/0bchQjlaVCbloi88lppDGBsV2HI=/0x0:3200x1800/1200x800/filters:focal(1344x644:1856x1156)/cdn.vox-cdn.com/uploads/chorus_image/image/63081289/draftniks_nba_draft_1_getty_ringer_4.0.jpg)

This project attempts to leverage Machine Learning in python to create effective predictions for the next batch of NBA Rookies.
## 2019 College Clustering
The first file posted on this project gives a very top down view of the college stats of the players entering this years draft from college. Player data is visualized with a correlation matrix and cluster analysis to better understand the statistical distribution of players in this draft, and to look for certain similarities. The correlation matrix shows how strongly similar two varibles are just within the world of college stats. From there, the variables were decomposed, and three different methods of clusterings were employed. These three clustering methods were K-Means,Agglomerative, and Affinity Propagation, and they all all helped with visualizing similarities and overarching patterns.
## College and Rookie Trends
This file examines how the game of basketball has changed from various statistical standpoints as presented by the datasets involved. This part of the project is split into two main sections: the evolution of College Stats and the evolution of NBA Rookie Stats. The College Stats section was examined over the timeframe of 2001-2019, and it was in turn broken down on the basis of points, assists, rebounds, and the ratio of 3 point attempts to 2 point attempts. There were no obvious statistical trends in these categories, but some outliers definitely poked out. Next up, NBA Rookie seasons were assesed on the same categories plus fantasy value on the timeframe of 1981-2019, and this proved to be more interesting. Although no strong trends were found on the categories of points, rebounds, and assists, there were definitely strong upward trends for all the categories related to 3 point shooting. The box plots for the 3 subcategories that fall under 3 point shooting really catpture the essence of the history and popularity of the 3 point shot (especially in the modern era). Finally, the fastasy value of different rookies were examined based on fantasy guidelines on NBA.com.
## Full College Clustering
Similar to the 2019 College Clustering, this file attempts to look at the college stats of all incoming rookies in the last 20 years. A correlation matrix was constructed to analyze basic feature similarities, and clustering algorithms were implemented to assess player similarities. Within the main objective of this project, Rookie Stats predictions, one main point of interest lied on what stats Zion Williamson would put up, given all the media commotion around him at the time of this project. One method of approaching this problem using clusters was to simply take the average of all the stats of the players in the same cluster as him. With this methodology, Zion Williamson is expected to average 14.16 Points, 8.54 Rebounds, 3.38 Assists, 0.96 Steals, and 0.8 Blocks in his Rookie season.
## Rookie Predictions
This file contains the core of the project, and it deals with everything from feature engineering and model hyperparameter tuning to the actual predictions for the 2019 Rookie Class. For feature engineering, a lot of experimentation was done with regard to the manipulation of the two categorical variables school and position (from variable dummification to simple integer mapping). A correlation matrix was constructed to see what features had the strongest impact on NBA specific stats, and sklearn's recursive feature elimination algorithm was appplyed to see what the top N most important features were. Those N features were then run through a variety of models that encompassed both tree based models (ex. extratrees, randomforrest, xgboost), and Neural Net models (ex. Feed Forward Neural Nets and LSTMs). The Vanilla feed forward NNs proved to be the most efferctive as they possesed the highest test r^2 and the lowest test mse. Once this model was selected, it was fine tuned and then run on the college data of the incoming rookie class. With this methodology, Zion Williamson is expected to average 14.32 Points, 6.72 Rebounds, 2.48 Assists, 1.46 Steals, and 0.84 Blocks in his Rookie season.

## Tools Used
Data Cleaning: BeautifulSoup, Pandas

ML Analysis: SkLearn, XGBoost, Keras, TPOT

Visualization: Matplotlib, SeaBorn, Plotly.js


*For this project, I had to webcrawl and webscrape data because there were no spreadsheets online that was extensive enough and structured to my liking. All the datasets I created for this project are now also available on Kaggle. (https://www.kaggle.com/siddhesvark/compiled-ncaa-basketball-data)

*For determining NBA Fantasy Value, and evaluating predictive Value in general, I used the new fantasy basketball scoring system provided by NBA.com (http://www.nba.com/article/2017/10/05/nba-unveils-new-official-fantasy-scoring)

*Interactive results were made with Plotly.js, and can be viewed on my Glitch. (https://nba2019rookiestats.glitch.me) 
