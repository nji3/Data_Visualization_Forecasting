# Data_Visualization_Forecasting
Performing the data visualization and forecasting tasks on different real-life dataset from the Internet.

## Dataset 1

The Zillow housing sale dataset is scraped from the internet. The code used for scraping is based on Chris Muir's files [ChrisMuir/Zillow](https://github.com/ChrisMuir/Zillow). Here I just collected the sales information in the area from zipcode 90001 to 90099O, which is mostly in around the Los Angeles area. The original file only contains very basic variables and for further analysis, more variables such as the Education and the Crime rate will be added in the future. 

### One important WARNING: Use the scarping code in ChrisMuir's repo at your own risk, scraping is against Zillow's TOC.

About using the scarping code, remeber to do several things to prevent the error:

In the terminal
```
pip3 install Selenium
pip3 install zipcode==3.0.1
pip3 install bs4
pip3 install lxml
```
