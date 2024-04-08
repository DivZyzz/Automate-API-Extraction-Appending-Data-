**# Automate-API-Extraction-Appending-Data-**
The code is automating the extraction of data from the CoinMarketCap API, appending the newly fetched data to an existing DataFrame, and includes some extra functionalities such as adjusting display options and analyzing trends over time. Here's a breakdown of how it achieves each aspect:

**Automate API Extraction:** The api_runner() function is responsible for fetching data from the CoinMarketCap API. It is designed to be called repeatedly in a loop to automate the extraction process. The loop runs api_runner() for 333 times with a sleep of 60 seconds between iterations, effectively automating the extraction process over a specified duration.

**Appending Data:** Within the api_runner() function, the fetched data is appended to an existing DataFrame (df). This ensures that each time the function is called, the new data is added to the DataFrame, effectively accumulating data over time.

**Extra Functionalities:**

**Adjusting display options:** The script adjusts pandas display options to show all columns (pd.set_option('display.max_columns', None)) and format float numbers (pd.set_option('display.float_format', lambda x: '%.5f' % x)).

**Analyzing trends over time:** The script computes mean percentage changes over various time periods for different cryptocurrencies, providing insights into their trends over time.

Overall, the provided code effectively automates API extraction, appends data to an existing DataFrame, and includes additional functionalities for analysis and visualization.
