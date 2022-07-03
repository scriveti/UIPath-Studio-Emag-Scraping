# UIPath-Studio-Emag-Scraping

Created a workflow using Community UiPath (Studio + Orchestrator) version to create several workflows that solves the following tasks:

Emag Scrapping Process 1:
- Navigate to emag.ro in laptops section sorted by the number of reviews (https://www.emag.ro/laptopuri/sort-reviewsdesc/c)
- Scrape the top 100 entries (including information about the product name, price, etc)
- Upload every laptop as a transaction in an Orchestrator Queue named “Laptops”

Emag Scrapping Process 2:
- Retrieve the data from the Orchestrator Queue
- Find the most expensive 3 laptops and compute the average price for all 100 laptops.
- Export the top 3 laptops in a CSV file that contains the laptop name and price.
