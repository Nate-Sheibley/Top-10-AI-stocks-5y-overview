# UCB-Data-Proj1-G3
UCBerkeley-Ext data analytics bootcamp Project 1

## Team Memebers 
* Nathan Sheibley
* Krissy Knight
* Dante Parcon
* Sabrina Linden
* Andrea Moncada
* Melissa Glover

# Project Summary: AI Companies vs. S&P 500 and Dow Jones
This project investigated the performance of top AI companies compared to established market indexes, the S&P 500 and Dow Jones, over the past five years (2019-2024).

We analyzed daily and cumulative returns, along with volatility (risk), to assess profitability and risk associated with each investment option. While some AI companies exhibited impressive growth, overall, there wasn't a significant difference in returns between AI companies and the market indexes. Additionally, despite higher volatility in some AI stocks, the overall risk profile wasn't demonstrably lower compared to the indexes.

Conclusion: Our findings suggest that AI companies, while promising, haven't consistently surpassed the market indexes in terms of returns or risk reduction. Therefore, we failt to reject the null hypothesis, which stated there would be no significant difference between AI companies and the indexes.

Link to the Power Point Presentation: https://docs.google.com/presentation/d/18OrJYFomjt88RlA2M-8i7M9ukaBOeqgP/edit#slide=id.g2e5b37fad8a_2_9 


# Question of interest and the hypothesis
 
### Question
Does the growth of AI stocks in the last 5 years suggest that investing in these companies is significantly more profitable than investing in most other companies based on the market indexes?
### If-Then
If I invest in the top AI companies, then I will see better profit compared to the market indexes, because there is a significant difference in the growth of these stocks and the market indexes.
### Null Hypothesis
There is no significant difference between the growth of AI stocks and the market indexes, as determined by average daily return year over year from 2019-2024, as compared to the S&P 500 or DOW.
### Alt Hypothesis
There is a significant difference between the growth of AI stocks and the market indexes as determined by average daily return year over year from 2019-2024, as compared to S&P 500 or DOW.
 
# Stock Performance Visualization
 
Analyzing stock performance involves multiple factors. In this project, we used a simplified approach based on parameters such as average stock prices, daily and cumulative returns, and volatility.

### Variables of interest:
Daily Average and Cumulative Returns: Indicators of a stock's performance over specific periods.
Volatility (Standard Deviation): Measures stock risk. Higher deviation indicates higher risk.
Risk Levels Based on Standard Deviation (STD):
Low risk: <10% STD
Medium risk: 10% ≤ STD < 20%
High risk: ≥20% STD
Now, let's move on to the graphs that illustrate these concepts in the context of our analysis.
 
### Plots:
 
A. Bar graph of average cumulative return for AI companies 2019-2024
![Bar graph of average cumulative return for AI companies 2019-2024](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/Average_Cumulative_Returns_2019-2024.png?raw=true)

This bar graph on the right shows an average cumulative return of each stock during 2019-2024. It indicate that some AI companies outperformed S&P 500 and Dow Jones,while others under performed
 
B. Line graph of average daily returns for AI companies 2019-2024
![Line graph of average daily returns for AI companies 2019-2024.](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/Average_Daily_Returns_2.png?raw=true)

C. Cumulative daylie returns for index ETFs and AI average
![Cumulative daylie returns for index ETFs and AI average](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/cumulative_returns_all.png?raw=true)
 
D. Highlight: Line graph of average daily returns for AI companies in 2020
![Highlight: Line graph of average daily returns for AI companies in 2020](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/Average_Daily_Returns_2020.png?raw=true)

This is a snapshot to show the situation during Covid-19 and how all stocks went down in March 2020, when lockdown started.

E. Line graph of average daily returns with volatility error bars to display the variance
![Line graph of average daily returns with volatility error bars to display the variance](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/average_daily_return_with_volatility_selected_symbols.png?raw=true)

This graph shows average daily returns with different colors indicating volatility (standard deviation) in %. For the cleaner visualization of our data, we selected the 2 the most and 2 the least volatile companies, as well as S&P 500 and D
The S&P 500 and Amazon have the lowest volatility, making them the safest investment options. 
AI and Tesla have the highest volatility among the analyzed stocks. But overall, all these stocks with an exception AI have low risk (below 10%). This shows no significant advantage of AI companies compared to S&P 500 and Dow Jones regarding risk assessments.

 
### Statistical testing and visualization 
 
Violin Plots to display the distributions

![Daily returns averaged over all years for the AI companies](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/Box_and_violin/violin_plot_AI_sep_all_years.png?raw=true)

Violin plots to visualize the distributions in an intuitive manner and suggest the ANOVA results. In lightof the AVONA testing, Nvidia is different from Amazon and Meta, which is not obvious from this plot. PATH and AI were removed from the ANOVA testing as the data was not the same length as the other stocks, unbalanced.


Daily returns per year for AI companies averaged together, then plotted next to the indices (SPY, DOW, INDU). 

![AIStocksProject/Plots/Box_and_violin/violinplots_aimerged_year_by_year_small_limits.png](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/Box_and_violin/violinplots_aimerged_year_by_year_small_limits.png?raw=true)

Aggregated AI company daily returns compared per year with the indices. The distributions look different but the ANOVA test indicates they are not significant, but it is close. The critical value is 2.9 vs the F-statistic at 2.65. The p-value above 0.05 as well, indicating low confidence in rejecting the null hypothesis.
 
## Statistical Tests

Based on the plots above, it is questionable whether or not there is statistically significant different between the average daily returns from 2019 to 2024 among the AI companies and indices. However, a repeated measures ANOVA test will test us for sure whether this is the case. 
 
### Analysis #1: Repeated Measures ANOVA
 
Method: Repeated measures ANOVA is used to test the difference between means over time for multiple groups. We want to know whether there is a statistical difference in the average daily mean return between the top 10 AI companies and the indices from 2019 to 2024.
 
#### General Hypothesis

H0: all means are equal | Ha: at least one mean is different
 
Hypotheses|F-Statistic|Numerator DF|Denominator DF|P-Value
---|---|---|---|---
AI companies and indices|2.6513|5|15|0.0655
AI companies only|8.6322|5|35|0.0000

 
#### Conclusions: 

1. Fail to reject the null hypothesis. There is not enough evidence to suggest al difference between AI aggregate performance and indices ETFs
2. Reject the null hypothesis.
There is a significant difference in average daily returns per year across the
top AI companies.
 
###  Analysis #2: Post-hoc Pairwise T-tests

Method: Post-hoc pairwise t-tests are performed after a significant ANOVA test to see which mean pairs are driving the differences found among the groups. A Bonferroni adjustment is used to test for multiple comparisons, a necessary p-value adjustment when performing multiple tests.
 

Pairwise Post-hoc Tests|T-Test statistic|P-Value
---|---|---
AMZN & NVDA|-2.8266|0.0368
META & NVDA|-2.9126|0.0332

#### Conclusion: 

The t-test pairs showing a significant mean between 2019-2024 are between NVDA and AMZN and then NVDA and META.

## Additional Considerations
 
Plots:
![Average closing prices of each stock by year](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/Average_Closing_Prices.png?raw=true)


This line graph shows that the stock prices of most AI companies are below those of the S&P 500 (SPY symbol) and above those of the Dow Jones Industrial Average (DOW symbol). 

The prices of AI companies appear to fluctuate more compared to the S&P 500 and the Dow Jones. This indicates that for conservative investors, AI companies may not be the safest investment option.


![Average closing prices over time (last 5 years)](https://github.com/Nate-Sheibley/UCB-Data-Proj1-G3/blob/main/AIStocksProject/Plots/average_closing_prices_over_time.png?raw=true)

Average closing price of each stock/index during 2019 - 2024. The previous slide showed a line graph; this slide presents a scatter plot of the same information
