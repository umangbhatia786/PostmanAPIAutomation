# CountryREST API Postman Collection

The CountryREST Postman Collection is a comprehensive suite designed to interact with a RESTful API that provides information about countries. This collection includes various requests to retrieve country details based on different parameters such as name, code, capital city, language, and region.

## Collection Details

- **Collection ID:** [b4e110fd-0684-40bd-80b9-0d6eca4cac6e](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#3%2C19-3%2C19)
- **Collection Name:** Countries
- **Schema Version:** [v2.1.0](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- **Postman Collection Link:** [View Collection](https://www.postman.com/martian-shuttle-783921/workspace/recipeapi/collection/25156113-b4e110fd-0684-40bd-80b9-0d6eca4cac6e?action=share&creator=25156113&source=collection_link)

## Requests Included

1. **Get All Countries**
   - Method: GET
   - URL: `{{baseURL}}/all`
   - Tests: Verify response status code is 200 and the presence of non-empty name fields.

2. **Get Country by Name**
   - Method: GET
   - URL: `{{baseURL}}/name/{{countryName}}`
   - Tests: Verify response status code is 200, presence of [tld](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#108%2C24-108%2C24) array, and set values for country-specific variables.

3. **Get Country by Code**
   - Method: GET
   - URL: `{{baseURL}}/alpha/{{countryCode}}`
   - Tests: Verify response status code is 200, country name, capital city, country code, language, and currency.

4. **Get Country by Capital**
   - Method: GET
   - URL: `{{baseURL}}/capital/{{capitalCity}}`
   - Tests: Similar to "Get Country by Code".

5. **Get Countries by Language**
   - Method: GET
   - URL: `{{baseURL}}/lang/{{language}}`
   - Tests: Verify response status code is 200, check if input country exists in the response, and each country name is a non-empty string.

6. **Get Countries by Region**
   - Method: GET
   - URL: `{{baseURL}}/region/{{region}}`
   - Tests: Verify response status code is 200 and that input country exists in the list of response.

7. **Get Countries by Sub Region**
   - Method: GET
   - URL: `{{baseURL}}/subregion/{{subRegion}}`
   - Tests: Similar to "Get Countries by Region".

## Variables

The collection uses variables for dynamic request configuration:

- [countryName](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#59%2C37-59%2C37)
- [countryCode](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#217%2C78-217%2C78)
- [language](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#220%2C26-220%2C26)
- [currency](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#81%2C42-81%2C42)
- [capitalCity](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#337%2C36-337%2C36)
- [callingCode](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#83%2C42-83%2C42)
- [region](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#84%2C42-84%2C42)
- [subRegion](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#85%2C42-85%2C42)

## Running the Collection

To run this collection, import it into Postman, set up your environment with the appropriate [baseURL](file:///Users/ubhatia/Documents/PostmanAPIAutomation/CountryREST/country.postman_collection.json#39%2C16-39%2C16), and execute the requests. Ensure to configure the variables as needed for specific requests.

## Contributing

Contributions to this collection are welcome. Please follow the standard GitHub pull request process to propose changes.

## License

This Postman Collection is available under the MIT License.

