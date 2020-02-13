<a href="../2. Data Processing">Back to Data Processing</a>

# Loading
***Resources:*** 
* <a href="https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Cheat+Sheets/Importing_Data_Python_Cheat_Sheet.pdf">DataCamp Importing Cheat Sheet</a>
* <a href="https://pandas.pydata.org/pandas-docs/stable/reference/io.html">Pandas Input/Output</a>
* <a href="https://www.freecodecamp.org/learn/">Free Code Camp - Responsive Web Design (HTML)</a>
* <a href="https://www.rithmschool.com/courses/html-css-fundamentals">Rithm School - HTML& CSS Basics</a>

## Pandas
This will be your bread and butter when it comes to loading (and manipulation). Think of this as your first stop when trying to load in a file. It has support for many different file types so if you cannot load a file in using Pandas... all I can say is good luck on whatever you're planning to do. 

All jokes aside, the most common file type you'll likely be dealing with will be `.csv`, so be very familiar with how to load it. 

## HTTP Requests / Web Scrapping
Urgh... Let me be frank, I don't like this section at all. However, it is still important to know as a data scientist. In order to perform this, quite a bit of knowledge on `HTML` is necessary (Elements, tags, attributes, classes, id, etc...). Some resources for learning `HTML` is listed at the top. 

Moving forward with the assumption you know some `HTML`, here is how we can perform a basic web scrapping
```
import requests
from bs4 import BeautifulSoup

url = "..."

r = requests.get(url)

html_doc = r.text

soup = BeautifulSoup(html_doc)

# grab title
soup.title

# grab text (element)
soup.get_text()

# getting all hyperlinks 
soup.find_all('a')
```

This is the very basic of web scrapping. If you know this well, you can move on to building `spiders/crawlers'` to scour the internet via <a href="https://scrapy.org/">`scrapy`</a> package.  