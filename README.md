# MongoDB-Web-Scraping-Challenge-
Mars News/Mars Weather Data Analysis

![image](https://user-images.githubusercontent.com/112173540/208285204-b8d380fb-2a23-4709-8668-31454087f44a.png)

- This assignment consists of two technical products:

  - Deliverable 1: Scrape titles and preview text from Mars news articles. Optionally export the data into a JSON file or a MongoDB database.

  - Deliverable 2: Scrape and analyse Mars weather data, which exists in a table.

# part_1_mars_news.ipynb.
In this section we were asked to scrape the Mars NASA news site [Link](https://redplanetscience.com/) and inspect the page to identify which elements to scrape
1.  Create a Beautiful Soup object and use it to extract text elements from the website.
2.  Extract the titles and preview text of the news articles that were scraped. Store the scraping results in Python data structures as follows:
    - Store each title-and-preview pair in a Python dictionary. And, give each dictionary two keys: title and preview. An example is the following:

      {'title': "Mars Rover Begins Mission!",
            'preview': "NASA's Mars Rover begins a multiyear mission to collect data about the little-explored planet."}
  
3.  Optionally, store the scraped data in a file or database (to ease sharing the data with others). To do so, export the scraped data to either a JSON file or a MongoDB database. # [mars_weather.csv](https://github.com/GILEV0/MongoDB-Web-Scraping-Challenge-/files/10253324/mars_weather.csv)

# part_2_mars_weather.ipynb
Section 2 asked for an analysis of Mars weather data from https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html 
1.  Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. 
2.  Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
    - id: the identification number of a single transmission from the Curiosity rover
    - terrestrial_date: the date on Earth
    - sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    - ls: the solar longitude
    - month: the Martian month
    - min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    - pressure: The atmospheric pressure at Curiosity's location
3.  Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
4.  Analyse your dataset by using Pandas functions to answer the following questions:

    - How many months exist on Mars?
    - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    - Find the average the minimum daily temperature for all of the months.
    - Plot the results as a bar chart.
    - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    - Find the average the daily atmospheric pressure of all the months.
    - Plot the results as a bar chart.

5.  About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimate the result by plotting the daily minimum temperature.
