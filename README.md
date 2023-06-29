# Pizza Tracker API
This is a Rails API backend for tracking pizza in restaurants. It allows you to manage restaurants, pizzas, and the association between them. You can retrieve a list of restaurants, get details of a specific restaurant with its associated pizzas, delete a restaurant, retrieve a list of pizzas, and create associations between existing pizzas and restaurants.

## Getting Started
To get started, follow the instructions below.

### Prerequisites
Make sure you have the following installed on your machine:

Ruby (version 2.7.0 or higher)
Ruby on Rails (version 6.0.0 or higher)

### Installation
Clone the repository:

```
git clone <repository-url>
Install the dependencies:
bundle install
```

Set up the database:

```
rails db:create
rails db:migrate
```

(Optional) Seed the database with your owb sample data and Start the Rails server:
```
rails db:seed
rails server
```
The API will be available at http://localhost:3000.

### API Endpoints
The following endpoints are available in the Pizza Tracker API:

Restaurants
GET /restaurants: Retrieve a list of all restaurants.
GET /restaurants/:id: Retrieve details of a specific restaurant with its associated pizzas.
DELETE /restaurants/:id: Delete a restaurant and its associated restaurant pizzas.
Pizzas
GET /pizzas: Retrieve a list of all pizzas.
Restaurant Pizzas
POST /restaurant_pizzas: Create an association between an existing pizza and an existing restaurant.
Data Format
The API returns and accepts data in JSON format. 

### Validation
The RestaurantPizza model has a validation for the price attribute, which must be between 1 and 30.


## Contributing
Contributions to the Pizza Tracker API are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

### License
The Pizza Tracker API is open source and available under the MIT License.

