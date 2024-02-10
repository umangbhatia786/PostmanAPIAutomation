# GoRESTE2E Postman Collection

This README provides an overview of the GoRESTE2E Postman collection, designed for end-to-end testing of the GoREST API. The collection includes tests for creating, retrieving, and deleting users.

## Collection Information

- **Collection ID**: [50e9857c-bc3e-464d-b78e-a0b53b6c278f](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#3%2C19-3%2C19)
- **Collection Name**: GoREST
- **Schema Version**: [v2.1.0](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- **Postman Collection Link**: [View Collection](https://martian-shuttle-783921.postman.co/workspace/EcommerceE2E~7579da71-7fa0-467d-ba78-9c88d78d8053/collection/25156113-50e9857c-bc3e-464d-b78e-a0b53b6c278f?action=share&creator=25156113&source=collection_link)

## Tests Included

### 1. Create User

- **Method**: POST
- **Endpoint**: `{{goRestBaseURL}}/public/v2/users`
- **Authorization**: Bearer Token
- **Tests**:
  - Status code is 201
  - Verify JSON Schema of the response

### 2. Get User

- **Method**: GET
- **Endpoint**: `{{goRestBaseURL}}/public/v2/users/{{user_id}}`
- **Authorization**: Bearer Token
- **Tests**:
  - Status code is 200 or 404 (if user is deleted)
  - Verify that User Name, Email, and Gender returned are correct

### 3. Delete User

- **Method**: DELETE
- **Endpoint**: `{{goRestBaseURL}}/public/v2/users/{{user_id}}`
- **Authorization**: Bearer Token
- **Tests**:
  - Status code is 204

## Variables

- [user_email](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#35%2C38-35%2C38)
- [user_name](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#36%2C38-36%2C38)
- [user_gender](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#37%2C38-37%2C38)
- [user_id](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#81%2C42-81%2C42)
- [isDeleted](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#19%2C38-19%2C38)

## Usage

1. Import the collection into Postman.
2. Set up your environment with the necessary variables, including the [goRestBaseURL](file:///Users/ubhatia/Documents/PostmanAPIAutomation/GoRESTE2E/GoREST.postman_collection.json#112%2C16-112%2C16) and the Bearer Token for authorization.
3. Run the collection either through the Postman UI or using Newman in the command line.

For more detailed instructions on using Postman collections, refer to the [Postman Documentation](https://learning.postman.com/docs/getting-started/introduction/).

