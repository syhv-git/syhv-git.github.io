---
layout: project
type: project
image: images/forex-chart.jpeg
title: Forex trading
permalink: projects/forex-trading
# All dates must be YYYY-MM-DD format!
date: 2019-03-01
labels:
  - Forex Trading
  - MQL4
summary: My experience in creating indicators and auto-bot traders for the Forex Market
---

<img class="ui fluid huge image" src="../images/PL-indicator.jpeg">

In the Spring of 2019, I was introduced to foreign exchange market trading, Forex, through my parents. The Forex market is a global decentralized market where people are able to trade currency pairs, indices, metals, and stocks. I saw the potential, and learned the fundamentals, but with school, I was unable to dedicate a lot of time to trading. A year passed, and I found myself bored in quarantine, and decided to learn more about indicators and trading bots. After back-testing hundreds of indicators, and watching them in real time, I created an indicator which is a derivative of the Average True Range(ATR) indicator, with some calculation modifications and compounded with one hardcoded moving average. The light blue line is an exponential moving average from the standard indicator list provided in MetaTrader4, the platform which hosts the Forex market. This worked well for the metals market, but was unreliable for currency pairs and indices. I utilized this indicator, along with market analysis, to enter and exit trades, and overall, I had a 48% success rate. This may not seem like a good indicator, and there are definitely better out there, but the win-loss ratio I used allowed margin for profits.

MetaTrader4 is coded in the programing language, MQL4, and this language is used to build any software used in MetaTrader4. After finding some success with my remixed indicator, I wanted to see if I could create a trading bot, which would automate trades, using this indicator to send out trade requests. This is a frowned upon tactic, as the largest single-day market crash conducted by a private investor, was done through automated trading. A video on the "flash crash" of 2010 can be seen <a href="https://www.youtube.com/watch?v=_ZDEWVJan0s&ab_channel=BloombergQuicktake" target="_blank" rel="noopener noreferrer">here</a>. However, automated trading is something that is immensely difficult to do successfully. I was successful in creating a trading bot which worked well sometimes, and failed miserably other times.

The success rate of this bot was around 32%, and a would have blown out my account if I were doing this in the live market. A lot of problems were based around translating my own intuitions and aggregate analysis of the market into code. However, the entries of the bot were often headed in a good direction, but market reversals would end the trade as a loss. I then started testing this as an entry bot, where I would then exit the trades on my own analysis, and the success rate was right around 45%. While this may seem worse than just utilizing the indicator without the auto-trader, I would enter almost 3 times as many trades than I would have without the bot. Timing in trading is everything, and if the bot were able to enter me into a trade when I was unable to view the market, I would only have to focus on exiting the trade. Proper risk management is crucial to become a skilled trader as anyone can make a profiting trade as a one-off, but minimizing losses is how one maintains net profits.

Since creating these, I have tested other customized indicators, but ultimately, I want to wait until my knowledge of programing and statistics-based algorithms improve. While I have the source code, I decided not to include them here as I do not want to fall into legal troubles. Simply stating, ”this is not financial advice,” is not enough these days, and I do not wish for anyone to bankrupt themselves with tools I created.
