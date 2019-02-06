# Facebook Followers dataset
In this project, I aim at finding the relationship between social media interactions and the stock market. Specifically, I would like to conduct a cross-correlation analysis between the Facbook Followers data and New York Stock Exchange data to test whether both observables follow the same pattern. If so, I would like to use machine learning techniques, such as Feed Forward Neural Networks and Gaussian Processes, to estimate the lows and highs of stock prices for a particular company. My exploratory analyses on the Facebook dataset indicated that the variations of "Check Ins" counts has a periodic behavior. Focusing on the weekly variations of DisneyLand Check Ins, the pattern in social media interactions indicates that people's visit to Disneyland rises about January as well as the stock prices of Walt Disney Co. Additionally I have found that the yearly average of Talking About counts for WWE is decreasing, and for Netflix is increasing at a lower pace. It seems in the future, we might expect a decrease in the stock prices of Netflix. Is it because of other companies providing better services, eg. Amazon Prime, or Hulu through Spotify? 


Here are some preliminary research on Facebook Followers dataset:
## Correlation Matrix between Facebook data attributes
This correlation matrix shows the linear Pearson's correlation coefficient for the attributes of the Facebook Followers dataset. It indicates that the number of "likes" is more correlated with the number of "talking about". It means people who are really activate on social media, tend to talk more and participate in the discussions. Also, to state the expected, the number of "check Ins" is more correlated with the number of "were here".

<img src="https://github.com/mehdirezaie/Facebook/blob/master/figs/corrmax.png" width="500" height="300">



## Highest Volatility 
Let's look at the top five usernames in terms of number of likes, check Ins, talking about, and were here counts. Facebook and Youtube possess highest number of likes, which is kind of expected. Top three in terms of Check Ins counts belong to Disneyland!! It seems this company has done a good job in terms of attracting people.

<img src="https://github.com/mehdirezaie/Facebook/blob/master/figs/barplots.png" width="800">

### Weekly variations in Check Ins counts (My Favorite)
To understand the dynamic of the Check Ins counts, I look at the weekly Check Ins counts variations (eg. standard deviations) for three usernames, `Disneyland`, `Cedar Point`, and `Empire State Building`. The DisneyLand check Ins counts ramps up about January and decreases by the begining of the summer. Another interesting fact, Cedar Point is pretty crowded during the summer (not suprised??). In case, you are wondering about the big __Spike__ around May 2017 at the Empire State Building, it is when the building went red in support of 2017 AIDS walk in New York (read about it in the news at https://www.esbnyc.com/tower-lighting-2017-05-18-000000).

<img src="https://github.com/mehdirezaie/Facebook/blob/master/figs/checkins.png" width="800">

#### Comparison with Stock Market
Based on the analysis on Check Ins counts, I realized that Disneyland business comes to fruition starting about January each year. Looking at the NYSE data from https://www.marketwatch.com/investing/stock/dis, as shown in the following, we can see a similar pattern in the Walt Disney Co. stock prices. __As my main project, I would like to conduct a cross correlation analysis to quantify the potential correlation between Facebook Check Ins counts and the stock prices for Walk Disney Co., and train a Machine Learning model eg. Feed Forward Neural Network to predict the next lows and highs of Walt Disney Co.'s stock prices.__

<img src="https://github.com/mehdirezaie/Facebook/blob/master/figs/dis_nyse_stock.png" width="800">


## Monthly average in Talking About counts for TESLA, FORD, and CHEVROLET
Another interesting thing I find in the Facebook dataset is that Facebook users tend to talk more about cars around January. In the following figure, I am showing the monthly average of Taling About counts for three companies, `Chevrolet`, `Ford`, and `Tesla`. All three cases share the same pattern, rising about January. This indicates that car companies introduce their new car models in January, and dealerships try to offer really good deals to get their old models off the parking lots. Facebook users are talking about new models and the deals of last year's cars. It would be worthwhile to conduct a cross correlation analysis to quantitatively model the relationship between the stock prices of car companies and Facebook users' activities.

<img src="https://github.com/mehdirezaie/Facebook/blob/master/figs/cars.png" width="800">


## Yearly average of Talking About counts for NETFLIX and WWE
By looking at the yearly average of Talking About counts, I can see that people tend to talk less about WWE as they would do in the pase, and the rate that people talking about NETFLIX is decreased relative to the previous year (compare 2018 with 2017). I would be wondering if we see a fall in the NETFLIX stock prices in coming years. As a side experience, I have terminated my NETFLIX subscription, and I have been using Hulu through spotify. I wonder if other services, like Amazon Prime Videos or Hulu, could explain the trend seen in the Facebook data for NETFLIX.

<img src="https://github.com/mehdirezaie/Facebook/blob/master/figs/netflix_wwe.png" width="600">



The Jupyter notebook used to carry out these analyses is [here](https://github.com/mehdirezaie/Facebook/blob/master/FACEBOOK.ipynb). Should you have any questions about the specifics of the analyses, feel free to email me at medirz90@icloud.com.
