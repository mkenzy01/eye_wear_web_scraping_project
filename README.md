Web Scraping for Smarter Eyewear Choices

---

Brief Report on FramesDirect and Glassesusa Web Scraping Project

This project involved building a fully functional Python web scraper for the FramesDirect eyeglasses page using Selenium and BeautifulSoup. The objective was to scrape all available products from the target URL and extract the required data fields: brand name, product name, original price, and current price. The extracted data was then structured into a Python list of dictionaries, with additional support for export into CSV and JSON formats. In addition to the required fields, the script was extended to also capture the discount label and direct product link for each item, making the dataset more complete and useful.

One of the challenges encountered was that the product link only had the direct url for each glasses without the base url (framesdirect.com), so we had to llook for a way to bring the base url + the product url together. Another challenge faced was on the glassesusa.com. The site is very dynamic and using classing names are unreliable as they can be changed anytime and that will break our code.

Another challenge was identifying the correct HTML structure for each product and locating the exact tags containing the required fields. The page contains nested containers, so it was necessary to inspect the product tile structure carefully before extraction. The solution implemented was to carefully use the chrome browser inspect element feature, combined with jupiter notebook to ensure the selectors are accurate. This approach made the code more organized and easier to debug.

Overall, the project was successful in meeting the main objective of scraping FramesDirect product data using Selenium and BeautifulSoup. While Glassesusa is still pending due to limited time. The major challenges were related to dynamic page loading, locating the correct HTML elements, and handling missing values safely.
