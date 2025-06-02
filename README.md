# ADS-509-Project
# Disaster Tweet Classification & Topic Modeling

## Team Members
- **Davood Aein** (GitHub: @Davoodaein66) – Data Acquisition & Cleaning  
- **Tarane Javaherpour** (GitHub: @Tarane2028) – Topic Modeling & Comparative Analysis  

## Problem Statement
We aim to build a supervised binary classifier to identify whether a tweet refers to a real‐world disaster. Subsequently, we will apply an unsupervised topic modeling algorithm to the same corpus (ignoring labels) and compare how well discovered topics align with the “disaster vs. non‐disaster” categories.  

**Why It Matters:** Rapid, automated classification of tweets can assist emergency responders, NGOs, and government agencies in triaging incoming social‐media signals during disaster events.  

## Dataset & Acquisition
- **Source**: Kaggle “Disaster Tweets” dataset (only tweet IDs + binary labels).  https://www.kaggle.com/code/gunesevitan/nlp-with-disaster-tweets-eda-cleaning-and-bert/notebook
- **Rehydration**: We rehydrate tweet IDs via the Twitter API (v2) using Python (Tweepy). See `data_acquisition/rehydrate_tweets.ipynb`.  
- **Output**: `data_acquisition/raw_disaster_tweets.csv` containing full tweet text, timestamps, engagement metrics, and original labels.  

## Repository Structure
