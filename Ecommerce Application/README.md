# Ecommerce Application End-to-End Testing

This document outlines the end-to-end (E2E) testing setup for the Ecommerce Application using Postman. The collection includes various operations such as user authentication, product management, and order processing.

## Collection Details

- **Collection ID:** [9a5f140d-a79c-4660-a304-1915261288c9](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#3%2C19-3%2C19)
- **Schema Version:** `https://schema.getpostman.com/json/collection/v2.1.0/collection.json`
- **Postman Collection Link:** [E2E Collection](https://www.postman.com/martian-shuttle-783921/workspace/ecommercee2e/collection/25156113-9a5f140d-a79c-4660-a304-1915261288c9?action=share&creator=25156113&source=collection_link)

## Key Operations

### 1. User Authentication

- **Login:** Validates user credentials and returns a token for authenticated requests.

### 2. Product Management

- **Add Product:** Allows adding a new product to the catalog.
- **Delete Product:** Enables the removal of a product from the catalog by its ID.

### 3. Order Processing

- **Create Order:** Facilitates the creation of a new order with one or more products.
- **View Order Details:** Retrieves details of an order by its ID.

## Variables

The collection utilizes variables for dynamic data handling:

- [userMail](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#62%2C38-62%2C38): User's email address.
- [password](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#62%2C77-62%2C77): User's password.
- [token](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#147%2C19-147%2C19): Authentication token received upon login.
- [userID](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#161%2C20-161%2C20): User's unique identifier.
- [product_id](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#266%2C89-266%2C89): Unique identifier of a product.
- [order_id](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#262%2C42-262%2C42): Unique identifier of an order.
- [product_name](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#133%2C38-133%2C38): Name of the product.
- [product_price](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#129%2C15-129%2C15): Price of the product.
- [product_description](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#130%2C15-130%2C15): Description of the product.
- [country](file:///Users/ubhatia/Documents/PostmanAPIAutomation/Ecommerce%20Application/E2E_Ecommerce.postman_collection.json#426%2C19-426%2C19): Country from where the order is placed.

## Testing

Each request includes tests to verify the response status code, message, and schema validation ensuring the integrity of the application's functionalities.

## Usage

To use this collection:

1. Import the collection into Postman.
2. Set up environment variables as needed.
3. Execute the requests in the sequence of operations.

For detailed request and test script examples, refer to the collection JSON file.

