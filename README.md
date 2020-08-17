# Amazon Scraper : Scrape and extract products details from "Amazon.com" search results pages and return it in JSON format.

A simple amazon scraper to extract product details and prices from Amazon.com using Python Requests and Selectorlib library. 

Steps:
Note: You have install selectorlib and requests library before running.
This scraper only scrapes product from the first page of search results

1. Add Amazon Product URLS to [search_results_urls.txt](search_results_urls.txt)
2. Run `python3 searchresults.py`
3. Get data from [search_results_output.jsonl](search_results_output.jsonl)

## Example Data Format


### Search Results 
Each result would look similar

```json
{
    "title": "New ! Dell Inspiron i3583 15.6\" HD Touch-Screen Laptop - Intel i3-8145U - 8GB DDR4-128GB SSD - Windows 10 - Wireless-AC - Bluetooth - SD Card Reader - HDMI & USB 3.1 -Waves MaxxAudio Pro- Black",
    "url": "/Dell-Inspiron-i3583-Touch-Screen-Laptop/dp/B08173ZTJX/ref=sr_1_3?dchild=1&keywords=laptops&qid=1591584632&sr=8-3",
    "rating": "4.1 out of 5 stars",
    "reviews": "122",
    "price": "$472.00",
    "search_url": "https://www.amazon.com/s?k=laptops"
}
```