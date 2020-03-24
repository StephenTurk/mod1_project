# Module 1 Final Project

## Introduction

Beginning this project the first step was to find a focus for where to advice the stakeholders, Microsoft, with their move into the film industry. 

## Key Questions

1. Where to enter the market? (In box office vs streaming, domestic vs international)

2. At what financial level to enter the market? (large vs. small budget)

3. How to enter the market? (what genre show the biggest returns for the smallest investment?)



## Imports that are necessary for the notebook
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
import numpy as np

## The Data

yearly_rev_df = pd.read_csv('yearly_revenue_w_inflation.csv') The Numbers
observer_investment = pd.read_csv('observer_stream_investment.csv') The Observer
tn_movie_budgets = pd.read_csv('zippedData/tn.movie_budgets.csv.gz') The Numbers
imdbtb = pd.read_csv('zippedData/imdb.title.basics.csv.gz') IMDB
opus_data = pd.read_csv('OpusMovieData.csv') Opus data from The Numbers

## The Notebook

Using the student.ipynb Jupyter Notebook will take a reader in detail through my thought process, data cleaning and visualizations. Findings are sumerized below.

## Question 1
1. Where to enter the market? (In box office vs streaming, domestic vs international)

Here we see a significant decline in domestic box office revenues as well as a corresponding jump in spending on streaming services. Moving towards an international and streaming audience is recommended.

Used these data sets:
yearly_rev_df = pd.read_csv('yearly_revenue_w_inflation.csv') The Numbers
observer_investment = pd.read_csv('observer_stream_investment.csv') The Observer

## Question 2
2. At what financial level to enter the market? (large vs. small budget)

By looking at whether increasing film budgets resulted in increased revenue we found that a lower budget of $20,000,000 to $50,000,000 was recommended as increased budgets did not seem to correspond to increased percentage gain in revenue.

Data set: tn_movie_budgets = pd.read_csv('zippedData/tn.movie_budgets.csv.gz') The Numbers

## Question 3
3. How to enter the market? (what genre show the biggest returns for the smallest investment?)

We first looked at the IMDB database to see what films were the most common, but this data was only mildly helpful in recommending profitable films. Next using the opus data set we were able to view percentage gain and production budget compared to each movie genre. Horror, Concert/Performance and Comedy were the most profitable areas with the least intial investment.

