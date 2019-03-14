# Data_Visualization_Forecasting
Performing the data visualization and forecasting tasks on different real-life dataset from the Internet.

## Dataset 1

The Zillow housing sale dataset is scraped from the internet. The code used for scraping is based on Chris Muir's files [ChrisMuir/Zillow](https://github.com/ChrisMuir/Zillow). Here I just collected the sales information in the area from zipcode 90001 to 900990, which is mostly in around the Los Angeles area. The original file only contains very basic variables and for further analysis, more variables such as the Education and the Crime rate will be added in the future. 

### One important WARNING: Use the scarping code in ChrisMuir's repo at your own risk, scraping is against Zillow's TOC.

About using the scarping code, remeber to do several things to prevent the error:

In the terminal
```
pip3 install Selenium
pip3 install zipcode==3.0.1
pip3 install bs4
pip3 install lxml
```
## Dataset 2

The StockX Sale data of 'Yeezy' and 'Off-White X Nike' is from the [StockX data contest 2019](https://stockx.com/news/the-2019-data-contest/). It contains a random sample of the sale record from 2017/09 to 2019/02. For this contest, only one chart is allowed to submit with no more than 200 words description. The jupyter notebook here contains my chart for the contest.

The dataset has more than 90000 rows which makes it not a small dataset. There could be more visualization and even model fitting on it for future study.

## Dataset 3

Dataset 3 is the Vehicles information and price values from the CraigsList. The whole data is 187 MB which is beyond the 25 MB limited by Github. The dataset contains beyond 600000 rows of vehicles information and the vehicles are manufactured from 1900 to 2019. There are thousands of the missing values in the file.

The data visualizations are conducted and selected part of data is used to do the price prediction and statistics model building.

## Dataset 4

Dataset 4 is the Health Scores data of the employees from a company. The dataset contains about 19000 rows with the record of the employees health score for quarters of years. Some visualization and analysis are done for this dataset.
