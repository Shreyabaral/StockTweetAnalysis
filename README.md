Twitter, being the social post office of the internet ingests a lot of data via tweets which are short
messages exchanged between the users on the platform. Twitter since its inception has quickly gained
popularity as a quick message platform not only for individuals but also for companies and is heavily
used to send out quick updates be it on some advisory like weather updates from Environment Canada
or commute updates from TTC.
Hence, twitter is a one stop shop to get all the latest news on the stock market and use it to our
advantage, however the data is not straightforward and needs some processing before it can spill the
beans on the which stock is worth buying or selling.
We aim to clean the data for a few keywords such as bitcoin, gold, etc. and use the data for further
analysis.

Introduction
With vast available data from twitter, we are trying to do an Exploratory Data Analysis once we have
ingested, cleansed and restructured the data. We are trying to analyze the count for each keyword of
the tweets and the number of users that are using that keyword which might be used in either sense;
positive or negative sense which may affect if the cryptocurrency/stocks goes up or down.
While our analysis on the preliminary level we plan to further drill down on this in future scope of the
project.

Exploratory Data Analysis
To do this EDA, we use pandas, NLTK, Sklearn and Numpy to transform the data on which we will
perform our EDA.
Step 1: Import all the required libraries
Step 2: Read all 8 files into respective dataframes.
Step 3: We check the shape of the dataframes to make sure the column numbers are same across and
we are good to merge them.
Step 4: Merge all the dataframes into one dataframe named trade_df.
Step 5: We run some basic analysis on the dataframe and correct datatypes, drop URL columns, drop
duplicates.
Step 6: We apply a preprocessing function where we use regex to remove hashtags, spaces,
punctuations, non-English characters and then we remove URLs from the text, fix spellings.
Step 7: We tokenize and lemmatize the data and we start with our EDA.

Conclusions and Future Work
With our EDA we can conclude that tweets may have some influence over the market and tweets may
affect how a certain stock or currency performs on that day, while this is proactive there may also be
reactiveness after an event has occurred which may influence further on the market.
There is a strong need to further use the data and train a model coupled with sentimental analysis to
predict what kind of impact a tweet will have, and this utility will be one of the most useful utilities for
not only organizations but also individuals who are looking to trade in the market.
We plan to implement sentimental analysis as the next phase and further enhance with a classification
model such as Decision Tree and Random Forest.
