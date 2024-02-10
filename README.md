# Postman API Automation

This repository contains collections and configurations for API testing and automation using Postman. It includes end-to-end tests for various APIs, as well as mock requests for testing purposes.

## Collections

### 1. GoRESTE2E

- **Overview**: End-to-end testing of the GoREST API, including creating, retrieving, and deleting users.
- **Details**: [GoRESTE2E README](GoRESTE2E/README.md)

### 2. MockRequests

- **Overview**: Testing various API functionalities, including fetching course details and verifying response schemas.
- **Details**: [MockRequests README](MockRequests/README.md)

## Tools and Technologies

- **Postman**: For creating and running API tests.
- **Newman**: Command line collection runner for Postman.
- **Apache JMeter**: Used for performance testing and generating performance reports.

## Getting Started

To use these collections:

1. Install Postman from [the official site](https://www.postman.com/downloads/).
2. Import the desired collection into Postman.
3. Set up your environment with the necessary variables.
4. Run the collection either through the Postman UI or using Newman in the command line.

For more detailed instructions, refer to the README files within each collection's directory.

## Reporting

Performance testing reports can be generated using Apache JMeter. Configuration details for report generation can be found in `apache-jmeter-5.5/bin/reportgenerator.properties`.

## Contributing

Contributions to this project are welcome. Please refer to the contributing guidelines before making any changes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
