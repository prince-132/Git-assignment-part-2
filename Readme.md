# Country-Capital API

This repository houses the code for a Python and Flask-based API that returns the name of a country when a capital city is provided. The API is served using the ASGI server Uvicorn.

## Features

- Provides the name of a country based on a capital city.
- Utilizes Flask for API development.
- Served by Uvicorn for asynchronous communication.

## Installation

To get started with the `country-capital-api`, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-organization/country-capital-api.git
   ```
2. **Navigate to the project directory:**
  ```bash
  cd country-capital-api
  ```
3. **Create a virtual environment:**
  ```bash
  python3 -m venv venv
  source venv/bin/activate
  ```
4. **Install the required dependencies:**
  ```bash
  pip install -r requirements.txt
  ```

## Running the API

To start the API server locally, use the following command:
```bash
uvicorn main:app --reload
```
- The API will be available at `http://127.0.0.1:8000`.

## Usage

You can consume the API by sending a GET request to the following endpoint:
```arduino
GET https://example.com/country-capital/<capital-city>
```

### Example Request:
```bash
curl -X GET "https://example.com/country-capital/paris"
```
### Example Response:
```json
{
    "country": "France"
}
```

## Deployment

For deployment, ensure the following environment variables are set:

- `ENVIRONMENT` - Set to `production` for production environments.
- `PORT` - The port on which the server will run.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contributing

If you wish to contribute to this project, please fork the repository and submit a pull request.
For major changes, please open an issue first to discuss what you would like to change.
