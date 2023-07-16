# Trip Hotel Info Scraper

[![WebScraper Data Science](https://img.shields.io/badge/SeleniumBot-Webscraper-blueviolet)](https://github.com/your-username/webscraper-selenium)

The Trip Hotel Info Scraper is a Python project that allows you to effortlessly retrieve hotel information for your trip without the need to manually open webpages. It utilizes Selenium WebDriver to scrape hotel data from a website and presents the information in a table format with three fields: the name of the hotel, the price per night, and the score.

## Requirements

To run this project, you need to have the following installed:

- Python (version 3.6 or above)
- Selenium WebDriver for Python
- ChromeDriver (ensure it matches your Chrome browser version)

You can install the necessary Python packages using pip:

```
pip install selenium prettytable
pip install selenium
pip install requests
pip install 
```

## Usage

1. Import the required modules:

```python
import types
import typing
from selenium import webdriver
import booking.constants as cons
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as ec
import os
from selenium.webdriver.common.keys import Keys as keys
from booking.booking_filteration import booking_filter
import time
from booking.booking_report import booking_report
from selenium.common.exceptions import StaleElementReferenceException, NoSuchElementException
from prettytable import PrettyTable
```

2. Instantiate the `booking` class, which extends `webdriver.Chrome`:

```python
driver = booking(driver_path=r"PATH-TO-SELENIUM-DRIVER", teardown=False)
```

3. Utilize the provided methods to interact with the webpage and retrieve hotel information. For example:

```python
driver.land_first_page()
driver.cross_check()
driver.change_currency(currency=None)
driver.select_searchbar(place_to_go)
driver.enter_dates(checkin, checkout)
driver.booking_count_inc(adult, child=None, rooms=None)
driver.click_search()
driver.apply_filtration()
driver.report_results()
```

4. Adjust the code according to your specific needs, such as by customizing the search parameters or modifying the output format.

Please ensure that you have set up the necessary environment and installed the required packages before running the code.

## Contributors

- [kaif khan](https://github.com/shadofaxx1)

Feel free to contribute to this project by submitting bug reports, feature requests, or pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
