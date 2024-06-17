# Project Description

Look into AI stocks and performance compared to other indicator stocks. 

Predictions for continuation of trends: 

# Scope

Top 10 AI companies

2021 May - 2024 May

Top 10 AI stocks in kaggle dataset. 

Indicies - S&P 500, Dow Jones

Trends to analyse: cumReturns, daylieReturns, Volitility, Correlation to stock indicies

# Questions, hypothesis and graphs
## Question
Does the growth of AI stocks in the last 5 years suggest that investing in these companies is significantly more profitable than investing in most other companies based on the market indexes?
### If-Then
If I invest in the top AI companies, then I will see better profit compared to the market indexes, because there is a significant difference in the growth of these stocks and the market indexes.
### Null Hypothesis
There is no significant difference between the growth of AI stocks and the market indexes, as determined by average daily return year over year from 2019-2024, as compared to the S&P 500 or DOW.
### Alt Hypothesis
There is a significant difference between the growth of AI stocks and the market indexes as determined by average daily return year over year from 2019-2024, as compared to S&P 500 or DOW.


## Graphs:
  * Correlation to stock indicies w/ regression lines
  * A sampling of timer series (current, before boom, durring boom)
  * cumReturn graphs, w/ regression lines (yearly)
  * Correlation heatmap for AI stocks to see if all are similar
 
  * Comparison of individual AI companies  
  * graph of total trade price for each company and compare ratios (stacked bar? scatter?)

# Due Date Mon, June 17th

# potential Datasets

https://www.kaggle.com/datasets/vladimirmijatovic/ai-stocks 

https://polygon.io/ stock market API if we have additional stock data - only povides 2y historical data for free. No indicies data

https://www.alphavantage.co/ has historic indicies data. May be hard to get opening closing. 25 req daylie limit

https://marketstack.com/ has historic indicies data. May be hard to get opening closing. 100 req monthly limit

# Other documents

[Presentation](https://docs.google.com/presentation/d/18OrJYFomjt88RlA2M-8i7M9ukaBOeqgP/edit#slide=id.p1)


[Proposal presentation](https://docs.google.com/presentation/d/1obsYiXWAbRGAWllP_sEavF3oh-RH_DJd/edit#slide=id.p5)

[gDoc Proposal](https://docs.google.com/document/d/139RJ7I75FHh-fn9RsUAjRVN0J7TTHlilzZtuNa3ryxY/edit)



---
---

# Plan: Agendas and Action items

Target: Data processing done by Monday (10th) EOD

Target: Data cleaning and processing done by Wed (12th) EOD

Target: Plots done by Fri (14th) EOD

Target: Presentations done Sat (15th) EOD

Target: Practice presentation Sunday

## Meeting 5 Agenda


1. project story - outline presentation and assign slides
2. outline story in readme (similar to presentation)
3. how does hypothesis fit into a story we can tell
4. create new or modify existing power point presentation? 
5. check project tracker to verify if we have any outstanding plots and meet rubric requirements
  

### AI - outline

Task order | Story beat | presentor/slide maker
---|---|---
Hypothesis - fail to reject null (1 slide)| what we came into it expecting and thinking | Melissa 
Performance metrics (1 slide) | how we measured this, where we got the data |  Melissa 
Overlayed 2020 plot (1 slide) | Confirmation metric, can see covid effect in 2020 | Dante
culm return (2 slides/plots) | compare DOW and SPY to AI stocks| Andrea
Avg daily returns for each stock (1 slide) | introduce that AI stocks may not be a better investment | Dante
volatility (1 slide) | show AI stock has high volatility | Sabrina
anova stat (1 slide - table?) | hard stats to show AI is not different from indices, mention correlation plot exists| Nate
violin plots (2 slides/plots, AI seperate, AI combined w/ indices) | visualize hard stats intuitively | Nate
Avg closing price by year (1 slide/plot) | Stock prices go up, they all went up similarly, AI not necessaily overheated  as incidated by lower stock price|  Sabrina
Conclusion |reitterate fail to reject null, mention quidkly all the reasons why | Sabrina 
Q&A graphs | | 
correlation graph | Some stocks were good indicators of others, some were not, Year was a negative indicator of nearly all which tracks with the news cycles | Nate


## Meeting 4 Agenda
AI: adjust scripts to save 10y of data. Combine dataframes and save a master csv

AI: Write functions for calculations using kaggle data as template. Use slide 6-7 in presentation
cumReturns, daylieReturns, Volitility, Correlation to stock indicies, avg top AI stockprice

AI: Apply calculations to API datasets. Check there are not errors from mismatched dataset format

AI: hypothesis development - poposal presentation


## Meeting 3 Agenda

### To complete by start of meeting 3

AI-: Do API calls for S&P500 and DJ
Done
AI-: Clean kaggle data
Done
AI: Write functions for calculations using kaggle data as template. Use slide 6-7 in presentation
Incomplete
cumReturns

daylieReturns

Volitility

Correlation to stock indicies

avg topAI stock price

AI: Clean API data. Transform API data to match kaggle data

AI: Apply calculations to API datasets. Check there are not errors from mismatched dataset format

cumReturns

daylieReturns

Volitility

Correlation to stock indicies

avg topAI stock price

AI: Turn google proposal docs to read only



---

## Meeting 2 Agenda Jun 6 2024
AI: Build project tracker

AI: Find API for stock indicies (Dow Jones and S&P500)

Response: If can not find API by EOD Shift to 2 years of data and use polygon API. Target, complete current 2 years of analysis, if time, and API anllows expand backways in 2y increments


AI: Scope of stock metric APIs: 

Response: cumReturns, daylieReturns, Volitility, Correlation to stock indicies, avg topAI stock price

AI: Decide graphs

Response: 
  * Correlation to stock indicies w/ regression lines
  * A sampling of timer series (current, before boom, durring boom)
  * cumReturn graphs, w/ regression lines (yearly)
  * plot avg AIcumReturn to see if any have outlier performances
  * Comparison of individual AI companies  
  * graph of total trade price for each company and compare ratios (stacked bar? scatter?)
  * Correlation heatmap for AI stocks to see if all are similar

---

## Meeting 1 Agenda Jun 5 2024

Decide exact data/scope

Finish roadmap outline, write day-tasks

Get API keys

Make API calls

clean data. Come back with good data monday

### TODO - sort into tasks/scope as appropriate

* Share of AI companies in fortune 500

* Combine with fortune 500 or other indicator stock for general comparison

* identify avg prices changes per stock/index. compare vs avg ai trend (all companies). find outliers

* Look at stock evaluation metrics/indicators.
Dataset includes trading volume.

* Combine daylie data to weekly or monthly and average
Use  we want.

### Questions: 

does AI stock outcompete common investments.

Identify trend of SP500, treasury bonds, other indicator stocks, and AI companies since AI boom 
Use unemployment or other proxies for economy health?

AI boom when? Baseline by going back a few years from then

Were these stocks more resilient in economic turmoil (2020)

Were there outliers within AI companies

When would AI have been the best investment. Is it still?

PREDICTIONS

### Advise from instructors:

[Proposal presentation](https://docs.google.com/presentation/d/18OrJYFomjt88RlA2M-8i7M9ukaBOeqgP/edit#slide=id.p1)

[gDoc Proposal](https://docs.google.com/document/d/139RJ7I75FHh-fn9RsUAjRVN0J7TTHlilzZtuNa3ryxY/edit)
 
market data api - there's a whole bunch. Check free tiers

api market

marksetstack - 1y history

6-8 graphs for the whole project

what metrics. performance? volatility? correlations?  pick sub ranges

focus on most current data primary.

take a sample of the years? 1 year current. 1 year before boom. a sample of other years tbd.

