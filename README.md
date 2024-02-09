# User API

This code provides a basic RESTful API for managing users. It is built using Node.js and Express.js, and interacts with a MySQL database for data storage. The API supports operations for retrieving, creating, updating, and deleting user records, as well as searching for users by name.

## Setup

Before running the application, ensure you have the following dependencies installed:

- Node.js
- MySQL database
- npm (Node Package Manager)

To set up the application, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the project directory in your terminal.
3. Install the required npm packages by running `npm install`.
4. Set up your MySQL database and configure the connection parameters in a `.env` file. Refer to the `.env.example` file for the required environment variables.
5. Run the application using the command `node server.js`.

## Usage

Once the application is running, you can interact with the API using HTTP requests. Below are the available endpoints:

### Welcome Endpoint

- **GET /**: Returns a simple welcome message.

### User Endpoints

- **GET /users**: Retrieves all users from the database.
- **GET /users/:id**: Retrieves a user by their ID.
- **POST /users**: Creates a new user.
- **PATCH /users/:id**: Updates an existing user partially.
- **DELETE /users/:id**: Deletes a user by their ID.
- **GET /users/search/:name**: Searches for users by name.

### API Documentation

The API documentation is available via Swagger UI. You can access it by navigating to `/api-docs` in your browser after starting the server.

## Dependencies

- **express**: Fast, unopinionated, minimalist web framework for Node.js.
- **mysql2**: MySQL client for Node.js with Promise support.
- **cors**: Middleware for enabling CORS (Cross-Origin Resource Sharing).
- **dotenv**: Loads environment variables from a `.env` file into `process.env`.
- **swagger-ui-express**: Middleware for serving Swagger UI documentation.
- **swagger-jsdoc**: Generates Swagger/OpenAPI specification for the API.



