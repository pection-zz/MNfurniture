## Fields

The scraper will extract the following fields

-   Product Name
-   Price Range
-   Product Image
-   Link to Product
-   Minimum Order
-   Seller Name
-   Seller Response Rate
-   Number of years as a seller on Alibaba

## Requirements

-   Python 3
-   Scrapy
-   Selectorlib

## Running the Scraper

1.  Add search keyword to [keywords.csv](https://github.com/pection/MNfurniture/tree/master/Program_python/Image-scraper/scrapy_image/resources/keywords.csv)
2.  Modify max_pages variable from [alibaba_crawler.py](Image-scraper/spiders/alibaba_crawler.py), to the maximum number of pages to scrape data from. The default is 5 pages.
3.  Run command `scrapy crawl alibaba_crawler -o out.csv -t csv` to get data as CSV into a file called out.csv or `scrapy crawl alibaba_crawler -o out.json -t json` to get data as JSON File.

## Learn more about the scraper

You can read more on how this scraper was built here <https://www.scrapehero.com/scrape-alibaba-using-scrapy/>
