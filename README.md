# Weather App

A lightweight weather dashboard built with HTML, CSS, and JavaScript. It lets users search for a city and view the current temperature, humidity, wind speed, and weather condition using the OpenWeatherMap API.

## Project Overview

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
│   └── wind.png
└── README.md
```

## How It Works

1. The user enters a city name in the search box.
2. When the search button is clicked, JavaScript sends a request to the OpenWeatherMap API.
3. The app reads the response and updates the weather card with:
   - city name
   - temperature
   - humidity
   - wind speed
   - weather icon
4. If the city is not found, an error message is displayed.

## Setup

### 1. Clone the project

```bash
git clone <repository-url>
cd "Weather"
```

### 2. Open the app

You can either:

- open `index.html` directly in your browser, or
- start a small local server from the project folder

Example using Python:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## API Configuration

This app uses a hardcoded API key in `main.js`:

```javascript
const apiKey = "YOUR_API_KEY";
```

If you want to use your own OpenWeatherMap key, replace the value in `main.js`.

> Important: keep API keys private and avoid committing them publicly if the project is shared online.

## Usage

1. Type a city name such as `London`, `Tokyo`, or `New York`.
2. Click the search button.
3. View the current weather information for that city.

## Notes

This is a front-end-only project and does not include backend logic, database storage, or user authentication.

## Future Improvements

- add a default city on page load
- support search by pressing Enter
- add 5-day forecast
- move API key to environment variables
- improve responsive design for mobile devices

## License

This project is provided for educational purposes.
