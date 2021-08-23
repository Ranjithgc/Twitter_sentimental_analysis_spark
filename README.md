# Twitter_sentimental_analysis

# TWITTER SENTIMENT ANALYSIS AND VISUALIZATION
start all spark servecies

$ ./sbin/start-all.sh
Import all necessary libaries

import tweepy import matplotlib.pyplot as plt from textblob import TextBlob import csv import time import os from dotenv import load_dotenv load_dotenv('.env')
create .env file for twitter secret keys and store them in it
Establish the connection

auth = tweepy.OAuthHandler(consumer_key,consumer_secret) auth.set_access_token(access_token,access_secret) api_connect=tweepy.API(auth)
fetch the data from twitter

tweet_data=api_connect.search('football')
write a python code to fetch the data and store in csv file with positive and negative tweet counts with help of textblob
write a code for visualization with necessary imports

import pandas as pd import matplotlib.pyplot as plt from matplotlib.animation import FuncAnimation %matplotlib

write code for bar chart as well as line chart for visualization of live count
