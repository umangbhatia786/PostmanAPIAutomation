# SOAPAutomation

SOAPAutomation is a Postman collection designed to automate the testing of a SOAP web service for temperature conversion. This collection includes tests for converting temperatures between Celsius and Fahrenheit.

## Features

- **Celsius to Fahrenheit Conversion**: Automates the process of sending a Celsius value and validating the Fahrenheit conversion.
- **Fahrenheit to Celsius Conversion**: Automates the process of sending a Fahrenheit value and validating the Celsius conversion.
- **Dynamic Value Generation**: Utilizes Postman's scripting capabilities to generate random temperature values for testing.
- **Validation**: Includes tests to validate the response status code and the accuracy of the temperature conversion.

## Collection Structure

The collection is structured into two main requests:

1. **CelsiusToFahrenheit**: Converts a given Celsius value to Fahrenheit.
2. **FahrenheitToCelsius**: Converts a given Fahrenheit value to Celsius.

Each request includes:
- A **prerequest** script to set up test data.
- A **test** script to validate the response.
