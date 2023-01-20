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
* Mars News: https://redplanetscience.com/
* Mars Temperature Data: https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html

### Methodology

The analysis and visualization involved scraping two websites related to news regarding Mars exploration and Mars climate data. 

The poject consisted of two parts:
* Part 1: Scrape titles and preview texts from Mars news articles. 
* Part 2: Scrape and analyze Mars weather data (table).

## Observations

Part 1 - Using a combination of Splinter and Beautiful Soup, we created a dictionary of all the articles available on the Mars News web page.  Developing the automation to collect all article data into a dictionary opens the door to organizing data and conducting further anaylsis, such as looking for trends or pulling specific elements of data.

Part 2 - After scraping the table containing temperature data for Mars, the following observations were made:

* There were 12 Martian months in the a Mars year
* The coldest and warmest months on Mars were Martian Month of 3 (-83.31°F) and 8 (-68.38°F) respectively.  Temperature data is presented in the table below. On average the temperature remains fairly stable throughout the Martian year.
<img width="687" alt="Screenshot 2023-01-18 at 8 47 07 PM" src="https://user-images.githubusercontent.com/115101031/213336362-db56e871-aa13-40c5-b738-d5469b60fdf7.png">

* Months with the lowest and highest atmospheric pressure on Mars were month 6 (745.05) and 9 (913.31) as presented in the table below. 
<img width="630" alt="Screenshot 2023-01-18 at 8 50 37 PM" src="https://user-images.githubusercontent.com/115101031/213336812-1dd91288-4700-4117-8150-a334b6a965f3.png">

## Conclusions
Web scraping provides many benefits for those who use it.
![image](https://user-images.githubusercontent.com/115101031/213495987-09267e8d-55fa-42a1-984c-6a4f84c163b0.png)

Source: https://raluca-p.medium.com/why-web-scraping-a-full-list-of-advantages-and-disadvantages-fdbb9e8ed010 

However, it also presents some challenges that can make effective data analysis difficult:
* Processing the extracted data through web scraping can be a time-consuming and energy-intensive process. This is because the information comes as HTML code and that can be difficult for some to read. Don’t worry, though, there is software that can take care of that too!
* Because websites’ HTML structures change regularly, your code needs to be constantly updated.
* Access and licensing may be limited for many sites, and can raise red flags for users.

When coupled with the powerful language and libraries of Python, web scraping is at it's peak performance:
* Web scraping alone is made increasingly difficult by the significant ubiquity of sites and platforms available. This is further complicated by new information added to the web every second. When built with any of the Python libraries (such as Beautiful Soup), the web scraper can automatically extract data from target sources every day. The code (usually in very few lines) only needs to be written just once for this to happen.
* Web scraping is a 2-part process that scrapes the necessary data in an unstructured format then parses or imports it in a structured format. A single Python web scraping script can easily/quickly handle both functions plus more. A web scraper built with Python can be written to scrape and append the data, then parse, import, and save it as a data frame and even visualize the extracted data with Matplotlib. A Python library like Beautiful Soup can be used to build a tool that effectively does this regardless of the amount of data involved.

Source: https://spenceraqason.medium.com/why-is-python-the-best-language-for-web-scraping-ec8482bb1432
