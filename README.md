# Overview
This repository contains the annotated dataset, the unigrams, bigrams and trigrams referenced in the paper **"The Longest Month: Analyzing the Dynamics of Opinions Regarding COVID-19 Vaccination from Tweets in the Month following the First Vaccine Announcement"** published in **IEEE Access**. The paper is available at https://ieeexplore.ieee.org/document/9354776 .

The tweets have been collected between **November 9, 2020** and **December 8, 2020** as described in our paper. On November 9, 2020, Pfizer and BioNTech have made the announcement regarding the 90% COVID-19 vaccine efficiency. One month later, on December 8, 2020 the COVID-19 vaccination has started in the UK.

> Note: The tweets have been minimally pre-processed before extracting the n-grams by removing stop words and duplicated white spaces.

Repository structure:
- dataset: contains a **balanced dataset** with **3249 tweets** annotated in the categories "against" (0), "neutral" (1) and "in favor" (2);
- n-grams-all: daily unigrams and bigrams+trigrams extracted from the dataset containing all the 2.349.659 tweets, sorted by the number of appearances;
- n-grams-cleaned: daily unigrams and bigrams+trigrams extracted from the dataset containing the cleaned tweets (duplicates and retweets have been removed), sorted by the number of appearances.

# Usage
In accordance with the Twitter policy, in the annotated dataset, only the tweet ids have been provided. The tweets can be hydrated using a tool such as Twarc (https://github.com/DocNow/twarc) or Hydrator (https://github.com/DocNow/hydrator).
