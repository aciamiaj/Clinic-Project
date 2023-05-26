# openfda-drug-api

The code provided in this repository demonstrates how to fetch data from the FDA Drugs API and perform search and filtering operations based on brand names and routes.

## API Base URL
The base URL for the FDA Drugs API is:
https://api.fda.gov/drug/drugsfda.json?api_key=KPgTDFke6AcBsKDMJugLGfJjGn5VjkBJzP3WHY7C

## Functionality
The code in this project provides the following functionality:
Search for drugs by brand name
Filter drugs by route
Usage
To use the Drug Search API, follow these steps:

Include the necessary JavaScript files in your HTML document.
<!-- Include the jQuery library -->
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>

<!-- Include the main JavaScript file -->
<script src="app.js"></script>
Use the searchBrand(url) function to search for drugs by brand name. Pass the API URL as the parameter.
searchBrand(`${baseUrl}&limit=99`);
Use the filterRoute() function to filter drugs by route. This function retrieves the selected route type and updates the API URL accordingly.

Use the resetRoute() function to reset the route filter. This function clears the selected route type and updates the API URL to retrieve all drugs.

Use the search() function to perform a search based on the value entered in the search field. The function retrieves the search query and updates the API URL to include the brand name in the search.

## Event Handling
The code provided includes event handlers for the following events:
keyup event on the search field: This event triggers a search after a short delay when the user stops typing.
click event on the filter route checkboxes: This event triggers a filter operation based on the selected route type.
click event on the reset route button: This event resets the route filter and retrieves all drugs.

## Dependencies
This project has the following dependencies:
jQuery library: Used for DOM manipulation and AJAX requests.
