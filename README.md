# fb_scraping
facebook, scraping, no API, API Developper

# Facebook Scraper Selenium

Scrape Facebook Public Posts without using Facebook API 

## What It can Do

- Scrape Public Post Text
    - Raw Text
    - Picture
    - Link
- Scrape Likes and Top 3 React Numbers
- Scrape Public Post Comments 
    - Links in Comments
    - Pictures in Comments

## Install Requirements

        pip install -r requirements.txt


## Usage

#### 1. Use scraper.py to print to screen or to file

```
usage: scraper.py [-h] -page PAGE -len LEN [-infinite INFINITE] [-usage USAGE]
                  [-comments COMMENTS]

Facebook Page Scraper

optional arguments:
  -h, --help            show this help message and exit

required arguments:
  -page PAGE, -p PAGE   The Facebook Public Page you want to scrape
  -len LEN, -l LEN      Number of Posts you want to scrape

optional arguments:
  -infinite INFINITE, -i INFINITE
                        Scroll until the end of the page (1 = infinite)
                        (Default is 0)
  -usage USAGE, -u USAGE
                        What to do with the data: Print on Screen (PS), Write
                        to Text File (WT) (Default is WT)
  -comments COMMENTS, -c COMMENTS
                        Scrape ALL Comments of Posts (y/n) (Default is n).
                        When enabled for pages where there are a lot of
                        comments it can take a while                        
```

Example: ```python scraper.py -page RochKaborePF -len 20 -usage WT```

#
The output is output.txt inside the script folder.
