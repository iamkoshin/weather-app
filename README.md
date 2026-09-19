# Weather App

A clean, responsive weather dashboard built with HTML, CSS, and JavaScript. It fetches live weather data from the OpenWeatherMap API and displays the current conditions for a city, including temperature, humidity, wind speed, and the relevant weather icon.

## Overview

This project is a simple front-end application that demonstrates:

- fetching live weather data from a public API
- dynamically updating the DOM with current conditions
- showing a friendly error message for invalid city names
- matching weather icons to the current condition

## Features

- Search for any city by name
- Display current temperature in Celsius
- Show humidity percentage
- Show wind speed in km/h
- Display weather icon based on condition
- Handle invalid or unknown city searches gracefully

## Tech Stack

- HTML5
- CSS3
- JavaScript (vanilla)
- OpenWeatherMap API

## Project Structure

```text
Weather/
├── index.html
├── main.js
├── style.css
├── images/
│   ├── clear.png
│   ├── clouds.png
│   ├── drizzle.png
│   ├── humidity.png
│   ├── mist.png
│   ├── rain.png
│   ├── search.png
│   ├── snow.png
│   ├── wind.png
│   └── weather-app.png
├── README.md
└── .git/
```

## Screenshot

![Weather App Preview](images/weather-app.png)

## How It Works

1. The user enters a city name in the search box.
2. When the search button is clicked, JavaScript sends a request to the OpenWeatherMap API.
3. The app reads the response and updates the weather card with:
   - city name
   - temperature
   - humidity
   - wind speed
   - weather icon
4. If the city cannot be found, the app shows an error message instead of the weather data.

## Setup

### 1. Clone the project

```bash
git clone <repository-url>
cd "Weather"
```

### 2. Run the app

You can either:

- open `index.html` directly in a browser, or
- serve the project locally

Example using Python:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## API Configuration

The app uses a hardcoded API key in `main.js`:

```javascript
const apiKey = "YOUR_API_KEY";
```

Replace the value with your own OpenWeatherMap API key if needed.

> Keep API keys private and avoid committing them to public repositories.

## Usage

1. Enter a city name such as `London`, `Tokyo`, or `New York`.
2. Click the search button or press Enter.
3. Review the current weather details for that city.

## Notes

This is a front-end-only project and does not include backend logic, database storage, or authentication.

## Future Improvements

- add a default city on initial load
- add animated weather transitions
- add a 5-day forecast
- move the API key to environment variables
- improve responsiveness for smaller screens

## License

This project is provided for educational purposes.
