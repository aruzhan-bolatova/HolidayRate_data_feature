This **HolidayRate** data feature provides a handy tool for travelers looking to **find the cheapest flights during holidays**. It leverages two powerful APIs, Calendarific and Amadeus, to achieve this:

- [Calendarific API](https://calendarific.com/): This API is used to fetch a list of holidays for a specified country and month. The notebook prompts the user to input the country and month they are interested in and retrieves the corresponding holiday data.

- [Amadeus API](https://developers.amadeus.com/self-service): This API is the backbone of the flight search functionality. Once the holidays are identified, the notebook uses the Amadeus API to retrieve flight information for each holiday date. This includes details like departure and arrival airports, flight dates, and, most importantly, the total price of the flight.

**Key Features:**

- Holiday-Specific Flight Prices: The tool retrieves flight prices specifically for the holiday dates, allowing users to see how prices fluctuate during these peak travel times.

- Price Comparison: Users can compare flight prices for different holidays within the same month to identify the most affordable travel dates.

- Normal Date Comparison: The tool also allows users to input a non-holiday date to compare flight prices and see the potential cost savings of traveling outside of holiday periods.

This data feature empowers travelers to make informed decisions about their travel plans, potentially saving them money by identifying cheaper flights during holidays.

**Future Improvements:**

- Adding a feature to automatically consider the next year if the selected month has already passed in the current year without a need to specifically input a year

- Customize Flight Offers: Number of passengers, Cabin class, Number of stops, Airlines

- Improve IATA Code Retrieval: The current method for obtaining IATA codes is scraping a website, which has errors in its data (i.e. Astana - 'TSE' is incorrect, should be 'NQZ').
Investigate alternative data sources for IATA codes. 

- Data Validation: Implement checks to ensure that the user inputs are valid, such as checking if the country code exists,validating the date format, confirming that the IATA codes are valid
