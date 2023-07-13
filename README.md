# Weather_Forecast_app
The main aim of this project is to provide users with real-time weather information, forecasts, and other weather-related data, which can help them make better decisions about their day-to-day activities.I built this project using HTML CSS & JavaScript. I’ve used OpenWeatherMap API to get the weather details of the user entered city or user’s current location.I used vanilla JavaScript to create this weather app. In the JavaScript file, I got the user entered city name and sent a get request to an OpenWeatherMap API with passing the city name. If the user clicked on the “Get Device Location” button then first I checked the user browser supports geolocation API or not.
# The HTML code  represents the structure of a weather dashboard application. It includes placeholders for weather data that will be populated dynamically using JavaScript. Here's a breakdown of the code:
The  head section includes the title of the page, a reference to an external CSS file (style1.css), and a reference to an external JavaScript file (weather.js).
The body section contains the main content of the weather dashboard application.
The h1 element displays the heading "Weather Dashboard".
The div class="container" element acts as a wrapper for the weather input and weather data sections.
The div class="weather-input" section includes an input field for entering a city name, a search button, a separator, and a button to use the current location.
The div class="weather-data" section contains the current weather and 5-day forecast sections.
The div class="current-weather" section displays the details of the current weather. The placeholders surrounded by underscores will be updated dynamically with actual weather data.
The div class="days-forecast"section displays the 5-day forecast. It includes an unordered list (ul) with five list items (li) representing each day's forecast. Similar to the current weather section, the placeholders within the list items will be updated dynamically with actual weather data.
The HTML code provides the basic structure of the weather dashboard, and the JavaScript file referenced in the script tag (weather.js) is responsible for fetching weather data and populating the placeholders with the retrieved data.


# The CSS code you provide adds styles to the HTML structure of the weather dashboard. Here's a breakdown of the CSS code:
The body selector sets the background image of the page using the background-image property.
The h1 selector styles the heading "Weather Dashboard" with a background color, font size, text alignment, padding, and text color.
The .container selector applies a flexbox layout to the container, sets the gap between its child elements, and adds padding.
The .weather-input selector styles the weather input section, including the input field, separator, and search buttons. It sets the width, height, font size, padding, margins, border, and background colors. The search button also has a hover effect.
The .weather-data selector styles the weather data section, including the current weather and 5-day forecast. It sets the width and color.
The .current-weather selector styles the current weather section, including the background color, border radius, padding, and flexbox layout.
The .current-weather h2 and .weather-data h6 selectors style the headings and details within the current weather section.
The .current-weather .icon and .current-weather .icon img selectors style the weather icon within the current weather section.
The .days-forecast h2 and .days-forecast .weather-cards selectors style the headings and weather card container within the 5-day forecast section.
The .weather-cards .card selector styles the individual weather cards within the 5-day forecast section. It sets the color, padding, list style, width, background color, and border radius.
Several @media queries are used to apply responsive styles at different screen sizes. The styles within these queries adjust the layout and sizing of elements for smaller screens.
Overall, the CSS code adds styling to the weather dashboard HTML structure, including backgrounds, colors, fonts, and layout adjustments for responsiveness.

# To make the weather dashboard functional and display actual weather information, you'll need to implement the JavaScript logic in the weather.js file. Here's a breakdown of the JS code:
The code defines several variables using document.querySelector to select elements from the HTML document. These elements include input fields, buttons, and div containers where weather information will be displayed.
The code sets the API_KEY variable to the updated API key for the OpenWeatherMap service. This key is necessary to make API requests.
The createWeatherCard function remains the same and is responsible for generating HTML code for weather forecast cards.
The getWeatherDetails function remains the same and is responsible for fetching weather data from the OpenWeatherMap API based on the provided latitude and longitude coordinates.
The getCityCoordinates function remains the same and is responsible for fetching the latitude, longitude, and name of a city based on the user's input.
The getUserCoordinates function remains the same and is responsible for retrieving the user's current location coordinates using the browser's Geolocation API.
Event listeners are added to the location button, search button, and city input field, just like in the previous code.
Overall, the code allows users to search for weather forecasts based on a city name or their current location and displays the forecast information in the HTML document. 
