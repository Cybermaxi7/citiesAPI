

# Cities API

This is a minimal JSON API for managing city data using [JSON Server](https://github.com/typicode/json-server). It provides basic CRUD (Create, Read, Update, Delete) operations on city resources.

## Getting Started

These instructions will help you set up and run the API on your local machine.

### Prerequisites

Before you begin, ensure you have [Node.js](https://nodejs.org/) installed on your system.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/cybermaxi7/cities-api.git
   cd cities-api
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the JSON Server:

   ```bash
   npm start
   ```

   The API will be available at `http://localhost:7000`.

## API Endpoints

The API provides the following endpoints:

- **GET /cities**: Get a list of all cities.
- **GET /cities/:id**: Get details of a specific city by ID.
- **POST /cities**: Create a new city.
- **PUT /cities/:id**: Update an existing city by ID.
- **DELETE /cities/:id**: Delete a city by ID.

### Example Usage

- Get a list of all cities:

  ```http
  GET http://localhost:7000/cities
  ```

- Create a new city:

  ```http
  POST http://localhost:7000/cities
  Content-Type: application/json

  {
    "cityName": "New York",
    "position": {
      "lat": 40,
      "lng": 0
    },
    "notes": "A great city!",
    "emoji": "🗽"
  }
  ```

## Contributing

If you'd like to contribute to this project, please follow these guidelines:

- Fork the repository on GitHub.
- Create a new branch for your feature/improvement.
- Make your changes and commit them with clear messages.
- Push your changes to your fork.
- Submit a pull request to the main repository.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

