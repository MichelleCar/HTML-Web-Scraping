# Mission to Mars: HTML-Web-Scraping
Exploring Mars on the World Wide Web!

![extraction](https://user-images.githubusercontent.com/115101031/213329422-63ae8cc0-0f00-4442-a786-197a9b199fa1.png)

## Background
Web sites are written using HTML, which means that each web page is a structured document. Sometimes it would be great to obtain some data from them and preserve the structure while we’re at it. Web sites don’t always provide their data in comfortable formats such as CSV or JSON.

This is where web scraping comes in. Web scraping is the practice of using a computer program to sift through a web page and gather the data that you need in a format most useful to you while at the same time preserving the structure of the data.

With so much information available to us online, it can be challenging to know where to start. Searching through pages and pages of content can be a time-consuming, sometimes fruitless endeavor. And even when you manage to do it, you might not get all the data you need. However, there is a common link between every web page on the internet; HTML, the code in which websites and web pages are written. To collect data en masse, you will need to deal with a lot of HTML code. That is why you need to scrape HTML data.

To put it simply, scraping is the act of taking data from the HTML code of websites and collecting it into one place for your personal use. The HTML code then gets broken down and separated according to the information that we want and require. Think of web scraping like hunting for rubies within a cave filled with treasures. The little pieces of information that you need are hidden gems within an overcrowded room. All objects in the room are treasures, but only a few are useful to you and your business. 

Source:
* https://docs.python-guide.org/scenarios/scrape/
* https://scrapingrobot.com/blog/html-scraping/

## Project Overview
This project focuses on web scraping and data analysis using Python libraries, Splinter, Chrome DevTools and many of its integrated useful modules, functions, and data structures while extracting and transforming various type of information.  To achieve our goals, we had to identify HTML elements on a page, identify their id, class, and other attributes, and used this knowledge to extract information through automated browsing with Splinter and HTML parsing with Beautiful Soup. These included HTML tables and news articles on a webpage. We then used the results to analyzing data, and posit insights of the datasets.

### Resources Used
Mars News: https://redplanetscience.com/
Mars Temperature Data: https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html

### Methodology

The analysis and visualization involved scraping two websites relevant to Mars exploration and Mars climate database. 

* Part 1: Scrape titles and preview texts from Mars news articles. 
* Part 2: Scrape and analyze Mars weather data (table).

## Observations

Part 1 - Using a combination of Splinter and Beautiful Soup, we created a dictionary of all the articles available on the Mars News web page.  Developing the automation to collect all article data into a dictionary opens the door to organizing data into a dataframe and further anaylsis, such as looking for trends and pulling specific elements of data.

Part 2 - After scraping the table containing temperature data for Mars, the following observations were made:
Number of Months on Mars

* There were 12 Martian months in the a Mars year
* The coldest and warmest months on Mars were Martian Month of 3 (-83.31°F) and 8 (-68.38°F) as presented in the table below. 
<img width="687" alt="Screenshot 2023-01-18 at 8 47 07 PM" src="https://user-images.githubusercontent.com/115101031/213336362-db56e871-aa13-40c5-b738-d5469b60fdf7.png">

* Months with the lowest and highest atmospheric pressure on Mars were Martian Month of 6 (745.05) and 9 (913.31) as presented in the table below. The lowest daily atmospheric pressure of 727.0 was recorded in Martian Month 6.
<img width="630" alt="Screenshot 2023-01-18 at 8 50 37 PM" src="https://user-images.githubusercontent.com/115101031/213336812-1dd91288-4700-4117-8150-a334b6a965f3.png">

* There are 3804 terrestrial (earth) days in a Martian year

