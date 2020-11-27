
1. Title: Popularity prediction of tweets 

2. Abstract
While the publication explores the general features of Twitter, we propose to predict the number of retweets that a tweet can have, thanks to supervised machine learning algorithms. This work could be interesting for newspapers or firms as it is important to them to be able to predict the popularity of a tweet. To do so, we propose to analyse the dataset to underline what is the part in the number of retweets taken by the date (hour, day, month and year), number of friends and followers, hashtags, urls, the language of the ego profile and mentions. Since the known number of followers of each ego is only known when the study has been made, the ego’s number of followers at the moment when some tweets  have been published could have changed, so we have to look into it to know how it could influence our prediction.

3. Research Questions
--> To what extent could the number of retweets of a given tweet be predicted ?
--> As we only know each ego’s number of followers at the moment of the study, how does it influence our prediction ?
--> Is the prediction reliable if we remove the number of followers from training labels ?

4. Proposed dataset

There are 3 dataset available with the original publication:

EgoAlterProfiles.txt
Mainly about the number of friends (user who mention each others usually) and followers for a given twitter account of the dataset

EgoTimelines.txt
A list of every tweet published by the twitter accounts of the dataset, with hashtag, date, number of RT, mentions, urls…

EgoNetworks.txt
A list of all the followers and followees for a given twitter account of the dataset.

We are interested in all the data related to the tweet’s  number of RT in order to train our algorithms. So we will merge the EgoAlterProfile and EgoTimelines in order to have an important overview of the accounts (with their relations and characteristics) and their tweet activity (with all the information for a given tweet). We may restrict our data to train our algorithm if an overfitting issue is present. Moreover, we may have to restrict the prediction to some periods due to lack of information, for instance we only have the measure of the number of followers in 2015.

5. Methods

--> Data collection and processing

--> Training of the algorithms

--> Testing of the prediction

6. Proposed timeline

Week 1: downloading all datasets available and cleaning them in order to get only information we need. Also process the data such as the date of publication of a tweet, so they could be used more easily.  Visualizing the influence of each parameter on retweet numbers to get a hint on what should be chosen as a feature for the prediction training. 

Week 2: implement the different learning methods that could be used for prediction. Try to predict the retweets count for each method. Analyzing the efficiency of these methods by calculating R² or accuracy scores and maybe visualizing their evolution depending on hyperparameters choice. 

Week 3: choosing the most effective method and doing a global analysis on its resulting predictions. In the meantime we will prepare the video and see if some points must be developed more and if some can be added.

7. Organization within the team

At the beginning one will focus on the different machine learning methods, one will clean the dataset and another one will pre process the data. Then when processing and cleaning  will be done, all members will focus their work on implementing predictive methods, maybe by working simultaneously on different ones. This will allow us to finally compare the efficiency of each method in order to have a great overall prediction.
The video will be done together, but each member will mainly present the steps and methods he worked on with regards to putting all the curves or tables useful to justify his foundings.




