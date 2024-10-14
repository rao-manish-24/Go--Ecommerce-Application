an e-commerce platform built using the Go programming language. 
It includes fundamental features such as user authentication, product management, and the integration of MongoDB as the database for storing product and user data. 
This platform is structured in a modular way, making it easy to extend and integrate more functionalities such as order management, payments, and inventory control in the future.

The application uses clean architecture principles to separate concerns, ensuring maintainable and scalable code.

Project Features
User Authentication: Handles user registration and login with password hashing.
Product Management: Includes endpoints to add, update, and retrieve product information from a MongoDB database.
Middleware: Implements authentication middleware to secure API endpoints.
MongoDB Integration: Uses MongoDB for persistent data storage, with separate collections for users and products.
Modular Design: Clean separation between API handlers, middleware, database operations, and data types.

Install dependencies:

The project uses Go Modules for dependency management. To download the necessary packages, run:
go mod tidy
Set up MongoDB:

Ensure MongoDB is running locally or remotely and set up a database for the application. The connection string should be specified in the environment variables.
Run the Application:

Use the Makefile to start the application:
make run
Alternatively, you can run the application directly using Go:

go run main.go
The server will be running at http://localhost:8080.
