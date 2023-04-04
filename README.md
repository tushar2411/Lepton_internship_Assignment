# Retail-Store-Location-Scraper
 Using web scraping techniques(such as requests and BeautifulSoup) to extract the store locations, store name, address, timings, coordinates(latitude/longitude), and phone number from the website.
Summary:

The Python script fetches JSON data by sending a POST request to a website URL, parses it and then stores the extracted data in a CSV file. The necessary modules such as requests, json and csv are imported, and the URL, request payload and headers are defined.

A POSTMAN application is utilized to obtain the header and payload information, which allows the testing of API requests and debugging of API endpoints. Using the requests module, the POST request is sent and the JSON data is retrieved. The JSON data is parsed with the json module and the required data is extracted.

Writing the data in the CSV file in the appropriate format is a significant technical challenge. Since the JSON response is a nested structure, the appropriate keys must be accessed using the Python JSON module. The csv writer object writes the required data in the correct format row by row.

Finding a website that enables data scraping while having all the necessary data is a non-technical challenge. Despite trying other websites such as Apple, Domino's Pizza and Taco Bell, the Unicorn Stores website is used. Unicorn Stores lacks store timings; however, as they are the same for all stores, the writer.writerow function is manually utilized to add the timings. Overall, using the correct Python modules and comprehending and manipulating data structures in the correct manner enabled the extraction and writing of the data in the correct format.
