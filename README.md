# Weather Forecast Minimal API

This is a simple .NET 8 (or later) Minimal API project that provides a basic weather forecast endpoint. It demonstrates the core features of a minimal API, including endpoint definition, dependency injection setup, and Swagger/OpenAPI integration for easy testing and documentation.

## Features

* **Weather Forecast Endpoint**: Generates a random 5-day weather forecast.
* **Minimal API**: Utilizes the streamlined API development model introduced in .NET.
* **Swagger/OpenAPI**: Automatic API documentation and a UI for testing endpoints (available in Development environment).

## Technologies Used

* **.NET 8 (or later)**
* **ASP.NET Core Minimal APIs**
* **Swagger/OpenAPI**

## Getting Started

### Prerequisites

* [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0) or later installed.

### Running the Application Locally

1.  **Clone the repository:**
    ```bash
    git clone <YOUR_REPOSITORY_URL>
    cd weather-forecast-api # Or whatever you named your repository
    ```
2.  **Restore dependencies:**
    ```bash
    dotnet restore
    ```
3.  **Run the application:**
    ```bash
    dotnet run
    ```
    The application will typically run on `http://localhost:5000` or `http://localhost:5001` (HTTPS).

### Accessing the API

Once the application is running:

* **Weather Forecast Endpoint:**
    * `GET /weatherforecast`
    * Example Response:
        ```json
        [
          {
            "date": "2025-07-16",
            "temperatureC": 25,
            "summary": "Mild",
            "temperatureF": 76
          },
          // ... more forecast items
        ]
        ```

* **Swagger UI (Development Only):**
    * Access the interactive API documentation at `http://localhost:5000/swagger` (or your specific port).

## Project Structure

* `Program.cs`: The entry point of the application, configuring services, defining the API endpoint, and running the app.
* `WeatherForecast.cs`: A record class defining the structure of the weather forecast data.

## Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is open-sourced under the [MIT License](LICENSE).
