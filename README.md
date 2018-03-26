# NCAA-Basketball-2018

One of our projects in the General Assembly Data Science Immersive program was to try to build a model to predict the NCAA Basketball tournaments. This coincided with the Kaggle competition called [Google Cloud & NCAA® ML Competition 2018-Men’s](www.kaggle.com/c/mens-machine-learning-competition-2018). As a long time sports fan and a multi-bracket per year maker, I was really excited to see to dive deep into this competition. Also, there is a cash price for the top three entries so that did not hurt either.

One of the biggest differences to this competition is that we must perdict the prbability of a team winning and predect on every possible game in the tournament. The competition is scored on who has the losest average log loss. An example on how it is scored is below. For more infromation I encourage everyone to check out the competition's website at the hyper-link above. 

IMAGE GOES HERE. 

# The Process

1. [Data Files](https://github.com/CBJohnson30/NCAA-Basketball-2018/blob/master/DataFilesInfo.ipynb)

- I knew this data was going to be clean it being a kaggel cometition so the first step was going to be exploring the data that was given to us. I loaded most of the CSV's given to us into a notebook to see what infromation was in each one. I would look at the columns, head and tail of each to get an idea on what data I was working this. While doing this I was thinking about how to tackel this. My first thought was to train my model on games that happened this year to predict games that might happen in the tournament. This is because college basketball changes so much from year to year and did not want old events to try to predict new outcomes. The data I was going to use from past years was school tournament history and years a coach has coached. The data I wanted from the current year included: yearly averages of box scores, rankings from major ranking systems and sport book futures which I would have to get from an online sports book. 
 
2. [Feature Extraction](https://github.com/CBJohnson30/NCAA-Basketball-2018/blob/master/Feature_extraction.ipynb)

- My next step was to pull the feaures out that I wanted and put them in a format that could be merged into one large DataFrame to be aable to train a model on. For each feature I created a function to pull it out or transform it from its orgional CSV then save it to a new CSV to use in my next step. This notebook was not only for features but to create a games list that I will be able to add featues to to be able to train a model. This included every game from every possible viewpoint. So it could be TeamA vs TeamB and TeamB vs TeamA eventhough the two teams only played once. 

3. [Joining Features](https://github.com/CBJohnson30/NCAA-Basketball-2018/blob/master/Joining_Features.ipynb)

- This was were I merged all of my featues into two large DataFrames that I could train a model on and predict on as well. One DataFrame was of the regualar season games and one was of every possible tournament game.  

4. [Models and Predictions](https://github.com/CBJohnson30/NCAA-Basketball-2018/blob/master/Model%20Testing%20and%20Predictions.ipynb)

- The last step was to start to build models and predict with them on the tournament games. 
 
