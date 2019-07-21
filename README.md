# twitter_profile_scraping_and_analysis
Wrangling and analyzing @dog_rates tweets

This repository contains my data wrangling and analysis project of the twitter.com/@dog_rates profile

The goal of this project was to extract data from 3 sources, wrangle and clean the data and ultimately pull out interesting observations from the data set. We analyzed the tweets from @dog_rates (https://twitter.com/dog_rates) which is an extremely popular twitter handle that post humorous dog photos and rate the dogs in a comical way. The tweets analyzed were from November 15, 2015 to August 1st, 2017.

I obtained my data from the following 3 sources:

Source 1: twitter-archive-enhanced.csv    - I obtained this file from Udacity, it can represent a file given by USB or stored in a company's directory.  

Source 2: image-predictions.csv           - This file was hosted on Udacity's website. I programmatically downloaded it. In future scenarios, if specific files are hosted on a website, instead of manually downloading them by visiting the website on Google Chrome or Mozilla Firefox, you can simply run a loop and quickly extract all the files you need.

Source 3: I scraped the required tweets from Twitter.com using the tweepy repository and Twitter's API. I collected the Favorite/Likes and Retweet Counts because this information was missing from the previous 2 files and it is very important.

The data was not clean and there were many steps that I had to do to obtain fair results. Some of the issues I had to fix were the following: 
- @dog_rates provides some fun ratings for the dogs. However, not all of these ratings were accuratly given to me so I had to scan the contents of all the tweets over again.  
- I also had to normalize the ratings as most but not all the ratings had a denominator of 10.
- Some of the dog names in the given files were completly wrong, I had to find these and change these values accordingly.

Visualizations for some of the findings are provided.

The main files for this project are the following:

1. wrangle_notebook.ipynb   - This file contains all the coding work
2. Wrangle_Report.pdf       - This file contains a quick summary of some of the toughest data quality/tidyness issues and how they were resolved.
3. Final_Report.pdf         - This file contains the results of the investigation.

License: You may freely use any part of my work/code.
