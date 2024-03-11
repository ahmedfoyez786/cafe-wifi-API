# Project Overview: Cafe & Wifi API
The Cafe & Wifi API is a RESTful api service designed to manage information about cafes, including their locations, amenities, and services such as Wi-Fi availability, seats, price etc. The API provides endpoints for searching cafes by location, retrieving random cafes, fetching all cafes, adding new cafes, updating coffee prices for existing cafes, and deleting cafes from the database.

# Database Management
The project utilizes an SQLite database to manage cafe information efficiently. SQLite is a lightweight, serverless relational database engine that stores data in a single file, making it easy to manage and deploy for small to medium-scale applications like this one.

# Technologies Used

* Python: Used for developing the API endpoints and handling requests/responses.
* Flask: A micro web framework for Python used to create the RESTful API.
* SQLite: The relational database management system used to store and manage cafe data.
* Postman: A popular API client used for testing and documentation.

# Cafe & Wifi API Documentation
### https://documenter.getpostman.com/view/33496881/2sA2xiVBSH
This API provides endpoints to manage cafes and their attributes such as location, Wi-Fi availability, and more.

## Base URL
http://127.0.0.1:5000

### Search Cafes by Location

- **Method:** GET
- **Endpoint:** `/search`
- **Description:** Search for cafes by location.
- **Parameters:**
  - `loc`: The location name to search for.


### Get a Random Cafe

- **Method:** GET
- **Endpoint:** `/random`
- **Description:** Get a random cafe from the database.


### Get All Cafes

- **Method:** GET
- **Endpoint:** `/all`
- **Description:** Get all cafes from the database.


### Add a Cafe

- **Method:** POST
- **Endpoint:** `/add`
- **Description:** Add a new cafe to the database.
- **Body Parameters:**
- `name`: The name of the cafe.
- `map_url`: URL to the location/map of the cafe.
- `img_url`: URL to an image of the cafe.
- `loc`: The location of the cafe.
- `sockets`: Whether the cafe has sockets (true/false).
- `toilet`: Whether the cafe has a toilet (true/false).
- `wifi`: Whether the cafe has Wi-Fi (true/false).
- `calls`: Whether the cafe allows phone calls (true/false).
- `seats`: The number of seats available in the cafe.
- `coffee_price`: The price of coffee in the cafe.

### Update Coffee Price for Cafe

- **Method:** PATCH
- **Endpoint:** `/update-price/{cafe_id}`
- **Description:** Update the coffee price for a specific cafe.
- **Parameters:**
- `new_price`: The new price of coffee for the cafe.


### Delete a Cafe by ID

- **Method:** DELETE
- **Endpoint:** `/report-closed/{cafe_id}`
- **Description:** Delete a cafe from the database by ID.
- **Parameters:**
- `api_key`: An API key for authorization.

## Copyright
© 2024 Foyez Ahmed



