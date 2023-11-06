# LLM-App
This respository contains my final project as part of the [10 Days Realtime LLM Bootcamp](https://ai-community-iitb-organization.gitbook.io/).

## Aim of the project
- This project is aimed at simplifying the process of the **querying and interpretation of analysis results** of daily stock market data of one or more stocks, making the process faster and more inuitive.
- The application aims to make the process of learning chart-reading analysis more interactive and enhances the learners intuition about the price action.
- An easy-to-use platform helps a person with no prior market experience develop the required skills for doing market analysis and help them transition more easily to sophisticated platforms (like [**Trading View**](https://in.tradingview.com/chart/)) for long-term investing or day-trading.
- Most such platforms have a cap of the number of indicators that can be simultaneously used on a graph, making a comprehensive analysis time consuming and tedious. Multiple indicator values can be queried at the same time, making the process much easier.
- The customizable **analysis.py** scripts offer users an opputunity to implement their own analysis parameters.

## How to use the project
- The ticker labels of the desired stock helps the script to fetch verified, *real-time* data (using **requests** and **BS4** modules) from a trusted sources (like [**Yahoo Finance**](https://finance.yahoo.com/) or [**NSE**](https://www.nseindia.com/)).
- A prior framework (based on **pandas** dataframes) is used to create the desired parameters, indicator values, and other relevant metrics and publish them to a csv file.
- This file is then formed into a vectorised format, which the user can query using the UI (built using **streamlit**) to help interpret and compare a lot of metrics at once, leading to a better result.
- Some sample queries -
> What are the current positions of the 20, 50 and 100 SMA as compared to the last closing price of the stock INFY
> 
> What are the values of the RSI, CCI and AO indicators
> 
> Give me the number of *dark-cloud cover* patterns were observed in the last month
