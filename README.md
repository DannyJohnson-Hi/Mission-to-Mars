# Mission-to-Mars
#### *HTML Web scraping on Mars data to create a Flask web application using Python and MongoDB*

## Overview
This project consisted on building a Python script to scrape text and images from various websites that talked about Missions to Mars. I then created a Flask web application, with a rendered HTML template designed using Bootstrap, to reflect data in certain locations w/o having to gather it all manually.

The data that was scraped and displayed, is stored in a non-relational Mongo database. furthermore, I attempted to connect the scraping script so that each time a button was clicked, the scraping would commence again, the database got updated, and new data was displayed. This button only works under the condition that these webpages don't change their HTML components I used for scraping. And lastly, by using Bootstrap's grid system I was able to create a responsive web app that could accomodate to any device people view it from. 

## Resources 
- Web pages scraped: 
  - https://spaceimages-mars.com
  - https://galaxyfacts-mars.com
  - https://marshemispheres.com/
- Software:
  - Python
  - Jupyter Notebook
  - Pandas, BeautifulSoup, Splinter, ChromeDriverManager, Flask, PyMongo
  - MongoDB
  - HTML5

## Summary


The final product was semi-functional web application built utilizing Flask that included images, a table with information about Mars in comparison to Earth, and the latest article title and short description scraped from the NASA's webpage. Each time we click on the "Scrape New Data" button new information should be updated on both the website and the MongoDB.


The scrape included a `news_title` with its brief explanation (`news_paragraph`), a `featured_image`, a table HTML component stored in `facts`, and four picture thumbnails, with their titles, of the different Mars' hemispheres stored in `hemispheres`. 

In addition, the database will be updated and each time new data is scraped it will be saved with a "last_modified" date to know when was the last time, as you can see in the bottom of the query results. In this case, it was on July 7th of 2021. 
