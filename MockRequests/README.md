# MockRequests API Collection

The MockRequests API collection is designed for testing various API functionalities, including fetching course details and verifying response schemas. This collection is hosted on Postman and can be accessed through shared links.

## Collection Information

- **Collection ID**: e729fead-5515-42e5-9e12-b6bc45b00887
- **Collection Name**: MockAPITestingCourses
- **Schema Version**: [v2.1.0](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- **Collection Link**: [View Collection](https://martian-shuttle-783921.postman.co/workspace/PostmanDemo~175059a1-ec4e-4001-90ac-ac7644cdd1b0/collection/25156113-e729fead-5515-42e5-9e12-b6bc45b00887?action=share&creator=25156113&source=collection_link)

## Endpoints

### 1. Get API Testing Courses

Fetches a list of API testing courses.

- **Method**: GET
- **URL**: `{{url}}/getapitestingcourses`
- **Response Example**:
```json
{
  "data": [
    {
      "course": "Postman",
      "price": 150,
      "category": "Javascript"
    },
    {
      "course": "SoapUI",
      "price": 25,
      "category": "Groovy"
    }
  ]
}
```

### 2. Get Course Details

Fetches details of a specific course by name.

- **Method**: GET
- **URL**: `{{url}}/getcoursedetails?name={{course}}`
- **Query Parameters**:
  - `name`: Name of the course
- **Response Example**:
```json
{
  "name": "postman",
  "category": "javascript",
  "content": "videos",
  "length": "15hours",
  "students": 12342
}
```

## Tests

The collection includes tests to verify the response status codes, content types, and specific data points like the number of students and course categories.

## Variables

- **url**: Base URL for the API endpoints. Current value: `https://029dc653-17f4-4720-83e4-b7564058599f.mock.pstmn.io`

## Usage

To use this collection, import it into Postman using the collection link provided above. Ensure to set the `url` variable to the base URL of the MockRequests API.

For more detailed instructions on importing collections and setting variables in Postman, refer to the [Postman Documentation](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/).
