# Data Analytics Capstone
##### By: Jordan Candido
##### Date Completed: July 16, 2022
## Outline
## ASK
### Choose a case study: 
#### Creating a investment information dashboard that contains price and stock information from a watchlist. Pull stock price data and other information from the Yahoo Finance API via a python script. The data is then cleaned and formatted before being placed into dataframes that export to .csv files. The .csv files are then imported into Power BI where the dashboard layout is creating showing visualizations including stock price charts and stock information tables/graphs. This project also pulls news article data from the NewsAPI API and performs sentiment analysis as well as natural language processing. 
### Identify the problem: 
#### Existing stock dashboards available on investment websites are generally good and provide specific benefits or powerful features that separate themselves from other. But these dashboards don't always show all the information that we are looking for and often times people use more than one website or dashboard to retrieve their information for investment decision making. The stock dashboard created in this project aims to present all the information that we look for when making investment decisions and will also be built upon as decision-making methods change or as new information is received. 
### Determine key stakeholders: 
#### Stakeholders for this project would include financial institutions such as banks, investment banks and government agencies as well as individuals that manage their own investments. 
### Explore the data and establish metrics:
#### The data is mostly comprised of historical price data and other financial metrics that have been tracked by the markets over the duration that a given stock has been publicly available. Other financial metrics include valuation metrics, business metrics, comparison metrics and more. The news article data targets and focuses on key words that are used multiple times within a given article. 
## PREPARE
### Collect data and store it appropriately: 
#### This project utilizes data from Yahoo Finance which is a popular and widely used website for investment information and their API is very easy to use and provides a lot of information that is used for fundamental and technical analysis. The API has many different functions that provide clean and formatted data that can be directly placed into a Pandas dataframe with only minor cleaning and preparation required before analysis or data export. The news article data is collected into a dataframe that contains all article information including title, source, text date and more.
### Identify how it's organized: 
#### The raw price data is organized in .json format in either a dictionary or a list for the information related to each ticker as well as the price data. A separate notebook was created to show the list of information available as well as the format it's in when it gets pulled in. Like the stock information data which also contains a lot of strings, the sentiment data would be classified as wide data with many columns for a short list of rows. 
### Sort and filter the data: 
#### The price data is sorted and filtered with a datetime index and includes price data in the format that is used for crating stock charts with columns for the High, Low, Open, Close and Volume. The specific financial metrics are provided in a list so this data is individually selected and pulled into a new column for each ticker in the watchlist. The news article text is filtered through using stop words that are not to be included in the analysis. These words including redundant words or words that do not provide much information or purpose by themselves. 
### Determine the credibility of the data: 
#### The data is provided and supported by financial markets and exchanges which have very accurate and complex systems that store all of the data for each ticker on their exchange. This data is also updated daily while the market is open and new data is recorded. The information provided is viewed as credible with no significant bugs or outliers present in the data when viewed and analyzed. The credibility of the news article data depreciates as time goes on because of the dates the articles are published on as well as the relevance or accuracy of the information. 
## PROCESS
### Check the data for errors: 
#### For specific tickers including ETF's, recently released tickers on public markets and other financial instruments may have Na or None values for certain data features. In these instances I used the .fillna() function to insert 0's or string data that matches the datatype of the column of data. 
### Transform the data into the right type: 
#### The data was transformed by formatting large monetary values into comma separated values, ratios into percentages and the string data did not require any cleaning or further preparation. 
### Document the cleaning process: 
#### Notes have been made within the code script to explain process and rationalization during the data gathering, cleaning and preparation process. 
### Choose your tools: 
#### The tools used in this script for data cleaning include the yfinance API, the requests library and the Pandas library which was used most in the cleaning and preparation phases of this project. For the sentiment analysis I used the nltk libraries for processing the text and words within the articles pulled for the NewsAPI. 
## ANALYZE
### Aggregate your data so it's useful and accessible: 
#### All price data was requested from the API and placed in dataframes that export to .csv files for each ticker and also a combined dataframe with all tickers in the watchlist with a datetime index and the closing price for each day. The financial metrics and other ticker information pulled from the API was added to a dataframe created from the original watchlist list that was used to pull all the stock data and was also exported to .csv format to use in the dashboard. 
### Organize and format your data: 
#### The dataframes themselves were created using camelcase format for consistency during scripting. The data in the dataframes including the columns and rows were formatted with capital titles for presentation purposes with the data itself formatted in an easy to read manor for accessibility when used in the dashboard. 
### Perform calculations: 
#### Calculation completed by converting ratio information into columns with a percent format.
### Identify trends and relationships: 
#### The data collected is used to create graphs and visualizations which help in identifying trends and relationships which guide the decision-making process for investing. 
## SHARE
### Determine the best way to share your findings: 
#### Due to issues with importing data to Tableau Public, I decided to learn and use PowerBI to present the investment data and visualizations. 
### Create effective data visualizations: 
#### The data visualizations include stock price charts, sector diversification, sentiment analysis and information tables. 
### Present your findings: 
#### See the PowerBI file or the notebook script to view the visualizations produced as part of this project. 
### Ensure your work is accessible to your audience: 
#### The data and visualizations were created with the aspects of readability and accessibility for the audience. 
## ACT
### Share next steps with your stakeholders: 
#### Information and insights gained in analyzing the data and visualizations impact the investment decision-making process where the investor decides whether or not to buy or sell a stock in the current market circumstances. 
### Determine if more data could give you new insights: 
#### More data could definitely enhance and support to purpose of this stock dashboard. I am motivated to keep working on this project for my own research and further improve my own investment decisions. 
### Upload to your portfolio: 
#### See the files in this GitHub repository or by using the link here: https://github.com/JordanCandido/Stock-Dashboard-Data-Analytics-Capstone.git 
