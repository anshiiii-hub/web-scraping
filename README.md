# web-scraping

A small Flask app that scrapes a practice bookstore ([books.toscrape.com](http://books.toscrape.com/)) and shows the results on a web page. Built while learning web scraping with Python.

## What it does

- `/` is the home page.
- `/books` fetches the bookstore's front page live and lists every book on it with its **title**, **price**, **availability** and **star rating**.
- If a field is missing it shows a placeholder instead of crashing, and if the request fails the page simply shows an empty list.

Nothing is cached: each visit to `/books` scrapes the site again.

## Tech

Python · Flask · requests · BeautifulSoup (`bs4`) · pandas (listed in `requirements.txt`)

## Run it locally

```bash
git clone https://github.com/anshiiii-hub/web-scraping.git
cd web-scraping
pip install -r requirements.txt
python app.py
```

Then open http://localhost:3000 and go to `/books`.

## Notes

[books.toscrape.com](http://books.toscrape.com/) is a sandbox site made for practising scraping, so this project is safe to run. It's a learning project, not a production scraper.
