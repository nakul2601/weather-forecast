# 10-Day Weather Forecast Website

A modern, responsive weather website that displays 10-day weather forecasts for any city worldwide.

## Features

- **Current Weather Display**: Shows current temperature, feels-like temperature, humidity, wind speed, and pressure
- **10-Day Forecast**: Detailed weather predictions for the next 10 days  
- **City Search**: Search for weather in any city worldwide
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI**: Beautiful gradient background with card-based layout
- **Weather Icons**: Emoji-based weather icons for better visual appeal
- **Loading States**: Smooth loading animations while fetching data
- **Error Handling**: User-friendly error messages for invalid cities or API issues

## Technologies Used

- **HTML5**: Semantic markup
- **TailwindCSS**: Modern CSS framework for styling
- **JavaScript (ES6+)**: Modern JavaScript with async/await
- **OpenWeatherMap API**: Real weather data provider
- **Font Awesome**: Icon library

## Setup Instructions

### Prerequisites

1. Get a free API key from [OpenWeatherMap](https://openweathermap.org/api)
   - Sign up for a free account
   - Navigate to the API keys section
   - Copy your API key

### Installation

1. **Clone or download the project files**
2. **Replace the API key**:
   - Open `index.html`
   - Find line 127: `const API_KEY = 'YOUR_API_KEY_HERE';`
   - Replace `YOUR_API_KEY_HERE` with your actual OpenWeatherMap API key

### Running the Website

1. **Option 1: Direct File Opening**
   - Simply open `index.html` in your web browser

2. **Option 2: Local Server (Recommended)**
   ```bash
   # If you have Python installed
   python -m http.server 8000
   
   # If you have Node.js installed
   npx serve .
   
   # Or use any other local server
   ```
   - Open your browser and navigate to `http://localhost:8000`

## Usage

1. **Default City**: The website automatically loads London's weather on page load
2. **Search for a City**: 
   - Type any city name in the search box (e.g., "New York", "Tokyo", "Paris")
   - Press Enter or click the "Get Weather" button
3. **View Weather Data**:
   - Current weather appears at the top with detailed information
   - 10-day forecast cards show below with daily predictions

## API Information

This website uses the OpenWeatherMap API:
- **Current Weather**: `/weather` endpoint
- **5-Day Forecast**: `/forecast` endpoint (used to generate 10-day view)
- **Units**: Metric (Celsius, m/s, hPa)
- **Rate Limits**: Free tier allows 60 calls/minute and 1,000,000 calls/month

## File Structure

```
weather-api/
├── index.html          # Main HTML file with embedded CSS and JavaScript
└── README.md          # This documentation file
```

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Features Breakdown

### Current Weather Section
- City name and country
- Current date
- Weather icon and description
- Temperature in Celsius
- Feels-like temperature
- Humidity percentage
- Wind speed in m/s
- Atmospheric pressure in hPa

### 10-Day Forecast Cards
- Day of the week and date
- Weather icon
- Daily temperature
- Weather description
- Humidity and wind speed

### Interactive Elements
- Hover effects on forecast cards
- Smooth transitions and animations
- Loading spinner during API calls
- Responsive search bar with Enter key support

## Troubleshooting

### Common Issues

1. **"City not found" Error**
   - Check the city name spelling
   - Try adding the country name (e.g., "Paris, France")

2. **API Key Issues**
   - Ensure your API key is correctly placed in the code
   - Verify your API key is active on OpenWeatherMap

3. **CORS Issues**
   - Use a local server instead of opening the file directly
   - Some browsers restrict API calls from `file://` URLs

## Future Enhancements

- [ ] Geolocation support for automatic location detection
- [ ] Weather alerts and notifications
- [ ] Temperature unit conversion (Celsius/Fahrenheit)
- [ ] Weather maps and radar
- [ ] Save favorite cities
- [ ] Dark/light theme toggle

## License

This project is open source and available under the MIT License.
