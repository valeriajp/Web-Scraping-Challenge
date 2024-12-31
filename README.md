# Web-Scraping-Challenge
# Background
You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their ![Screen Shot 2024-12-31 at 14 36 49](https://github.com/user-attachments/assets/0525cd6f-9f49-4bf3-9284-70206a442bce) and ![Screen Shot 2024-12-31 at 14 36 54](https://github.com/user-attachments/assets/24943295-9447-41ec-a47a-21c9e04e2f8e) attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights.
# What You're Creating
This new assignment consists of two technical products. You will submit the following deliverables:

    - Deliverable 1: Scrape titles and preview text from Mars news articles.
    - Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

# Instructions
# Part 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named ![Screen Shot 2024-12-31 at 14 40 06](https://github.com/user-attachments/assets/4666804e-f234-4a09-84eb-57bf076e1af3). You will work in this code as you follow the steps below to scrape the Mars News website.

 1. Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.
    HINT: To identify which elements to scrape, you might want to inspect the page by using Chrome DevTools.

  2. Create a Beautiful Soup object and use it to extract text elements from the website.

  3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

    - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: ![Screen Shot 2024-12-31 at 14 42 15](https://github.com/user-attachments/assets/db5ace9f-adfc-4704-970a-4fac218aea12) and ![Screen Shot 2024-12-31 at 14 42 21](https://github.com/user-attachments/assets/d30c4e7e-c361-4e17-8ffc-546f91ad560d). An example is the following:

![Screen Shot 2024-12-31 at 14 44 55](https://github.com/user-attachments/assets/797b6f8c-3860-41ca-a3dd-e6003e414624)

    - Store all the dictionaries in a Python list.
    - Print the list in your notebook.

  4. Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)

# Part 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named ![Screen Shot 2024-12-31 at 14 49 06](https://github.com/user-attachments/assets/da19342c-6d10-4061-82c7-f9e80696c32d). You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

  1. Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site. Inspect the page to identify which elements to scrape. Note that the URL is![Screen Shot 2024-12-31 at 14 50 06](https://github.com/user-attachments/assets/1c1eeaef-5722-423c-980a-b272ed758f60).
   HINT: To identify which elements to scrape, you might want to inspect the page by using Chrome DevTools to discover whether the table contains usable classes.
  2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas ![Screen Shot 2024-12-31 at 15 07 04](https://github.com/user-attachments/assets/afc4018c-696e-40ab-acbe-b5368468b65e) function. However,
     use Beautiful Soup here to continue sharpening your web scraping skills.
  3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
     - ![Screen Shot 2024-12-31 at 15 07 34](https://github.com/user-attachments/assets/662c97c4-f5be-47e3-ad3d-1e7b3dd10e36): the identification number of a single transmission from the Curiosity rover
     - ![Screen Shot 2024-12-31 at 15 08 40](https://github.com/user-attachments/assets/a7ccf8f2-f331-4df1-9986-31dcccd5388e): the date on Earth
     - ![Screen Shot 2024-12-31 at 15 08 40](https://github.com/user-attachments/assets/6dbc2131-4a51-4c7c-8e8e-f6590b7f835e): the number of elapsed sols (Martian days) since Curiosity landed on Mars
     - ![Screen Shot 2024-12-31 at 15 09 40](https://github.com/user-attachments/assets/11221857-3d26-4da2-aca1-f0da3511a167): the solar longitude
     - ![Screen Shot 2024-12-31 at 15 10 01](https://github.com/user-attachments/assets/eff190d0-eb0e-4e52-aef2-91a85e58315b): the Martian month
     - ![Screen Shot 2024-12-31 at 15 10 46](https://github.com/user-attachments/assets/416e8ab9-8cfd-498d-8fa5-0784747513b8): the minimum temperature, in Celsius, of a single Martian day (sol)
     - ![Screen Shot 2024-12-31 at 15 11 11](https://github.com/user-attachments/assets/fd9d7198-6684-4283-bdd2-cf13c6644efc): The atmospheric pressure at Curiosity's location
  
  4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate ![Screen Shot 2024-12-31 at 15 11 50](https://github.com/user-attachments/assets/14d010d3-3bb2-4bc0-b6c8-3fe460b35d0d), ![Screen Shot 2024-12-31 at 15 12 26](https://github.com/user-attachments/assets/4490c3c3-e4eb-4b9a-88a1-1fa0ea944fc0), or ![Screen Shot 2024-12-31 at 15 12 48](https://github.com/user-attachments/assets/e2f4bf10-9154-4b4d-84d0-4dd9e6ded94f) data types.
     HINT: You can use the Pandas ![Screen Shot 2024-12-31 at 15 11 50](https://github.com/user-attachments/assets/22f16713-f9e2-43e8-922b-5c074c782253) and ![Screen Shot 2024-12-31 at 15 14 12](https://github.com/user-attachments/assets/3df3fb88-e89d-46a2-8dd4-6818f72910f5) methods to accomplish this task.
  5. Analyze your dataset by using Pandas functions to answer the following questions:
     - How many months exist on Mars?
     - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
     - What are the coldest and the warmest months on Mars (at the location of![Uploading Screen Shot 2024-12-31 at 15.13.27.png…]()
 Curiosity)? To answer this question:
       - Find the average minimum daily temperature for all of the months.
       - Plot the results as a bar chart.
     - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
       - Find the average daily atmospheric pressure of all the months.
       - Plot the results as a bar chart.
     - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
       - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
       - Visually estimate the result by plotting the daily minimum temperature of each observation.
6. Export the DataFrame to a CSV file.

# Requirements
# Part 1: Scrape Titles and Preview Text from Mars News (40 points)
      - Automated browsing (with Splinter) was used to visit the Mars news site, and the HTML code was extracted (with Beautiful Soup). (10 points)
      - The titles and preview text of the news articles were scraped and extracted. (20 points)
      - The scraped information was stored in the specified Python data structure—specifically, a list of dictionaries. (10 points)

# Part 2: Scrape and Analyze Mars Weather Data (60 points)
      - The HTML table was extracted into a Pandas DataFrame. Either Pandas or Splinter and Beautiful Soup were used to scrape the data. The columns have the correct headings and data types. (15 points)
      - The data was analyzed to answer the following questions: (10 points)
          - How many months exist on Mars? (5 points)
          - How many Martian days' worth of data are there? (5 points)
      - The data was analyzed to answer the following questions, and a data visualization was created to support each answer: (30 points)
        - Which month, on average, has the lowest temperature? The highest? (10 points)
        - Which month, on average, has the lowest atmospheric pressure? The highest? (10 points)
        - How many terrestrial days exist in a Martian year? A visual estimate within 25% was made. (10 points)
      - The DataFrame was exported into a CSV file. (5 points)

# References
The Mars News websiteLinks to an external site. is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars NewsLinks to an external site. website in November 2022. Images are used according to the JPL Image Use PolicyLinks to an external site., courtesy NASA/JPL-Caltech.
