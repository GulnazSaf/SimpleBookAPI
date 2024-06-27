# Simple Book API

This file contains a Postman API collection that tests a positive end-to-end scenario.

## Installation and Running Instructions

1. Install Postman on your local machine.
2. Download the `.json` file from this repository.
3. Import the downloaded file into Postman.

You can now run the tests and verify the positive end-to-end scenario.

## API documentation

[Link to documentation](https://github.com/vdespa/introduction-to-postman-course/blob/main/simple-books-api.md)

## API Tests

**GET API Status**
  - Status code is 200
  - Status should be OK
  - Response time is less than 300ms
**GET List of book**
  - Status code is 200
  - Check all fields in each book object
  - Book found
  - Response time is less than 300ms
**GET Get a single book**
  - Status code is 200
  - Check all fields in response
  - Is in stock
  - Response time is less than 300ms
**POST API Authentication**
  - Status code is 201
  - Check all fields in response
  - Response time is less than 300ms
**POST Order book**
  - Status code is 201
  - Check all fields in response
  - Order is created
  - Response time is less than 300ms
**GET Get an order**
  - Status code is 200
  - Response has the required fields
  - Id is a non-empty string
  - Timestamp is a positive integer
  - Customer name in order is correct
  - Ordered book id is correct
  - Ordered quantity is correct
  - Response time is less than 300ms
**PATCH Update an order**
  - Response status code is 204
  - Response time is less than 300ms
**GET Get all orders**
  - Response status code is 200
  - Response time is less than 300ms
  - Content-Type header is application/json
  - Validate the order object schema
  - Validate the properties of the response
  - Customer name in order is updated
**DELETE Delete an order**
  - Status code is 204
  - Response time is less than 300ms
