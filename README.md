Weather Information App
Overview
The Weather Information App is a Java-based application that provides real-time weather updates for any location worldwide. The app uses the OpenWeatherMap API to fetch weather data, including temperature, humidity, wind speed, and conditions, and displays the information in a user-friendly graphical user interface (GUI). Additionally, the app offers a unit conversion feature and keeps a history of weather searches.

Features
Real-Time Weather Updates: Fetch and display current weather conditions for any location.
Unit Conversion: Switch between Celsius and Fahrenheit for temperature, and between km/h and mph for wind speed.
Weather Icons: Display weather condition icons fetched from the OpenWeatherMap API.
Search History: Keep track of previous weather searches and display them with timestamps.
Dynamic Background: The app changes its background color based on current weather conditions (e.g., clear, cloudy, rainy).
Getting Started
Prerequisites
Java Development Kit (JDK) 8 or higher
Internet connection to fetch weather data from the OpenWeatherMap API
Installation
Clone the repository or download the source code.

Compile the code using your favorite Java IDE (e.g., IntelliJ IDEA, Eclipse) or via command line:

bash

javac -d bin src/weatherapp/*.java src/*.java
This command will compile all the Java files and place the compiled classes into the bin directory.

Run the application:

bash
java -cp bin Main
Running the App
Launch the application by running the Main class.
Enter a location in the text field provided at the top of the window.
Click "Search" to fetch and display the weather data for the entered location.
Switch units by selecting either "Celsius" or "Fahrenheit" from the dropdown menu.
View the 8-day weather forecast (currently displaying mock data).
Check the search history at the bottom of the window.
Implementation Details
Class Descriptions
Main Class: The entry point of the application. It initializes and launches the GUI.

WeatherAppGUI Class: This class handles the GUI setup and user interactions. It includes components for location input, displaying weather data, and managing the search history.

WeatherAPI Class: Responsible for fetching weather data from the OpenWeatherMap API. It sends a request to the API and parses the JSON response.

WeatherData Class: A model class that stores weather data, including temperature, humidity, wind speed, and conditions.

WeatherHistory Class: Manages the search history, storing weather data associated with different locations.

UnitConverter Class: Provides methods for converting between Celsius and Fahrenheit, as well as km/h and mph.

WeatherIconManager Class: Fetches and returns weather condition icons based on the icon code provided by the API.

Key Functionalities
API Integration: The app integrates with the OpenWeatherMap API to fetch real-time weather data based on user input.

GUI Design: The GUI is built using Java Swing components. It is designed to be intuitive and user-friendly, with clear labels and a consistent layout.

Data Handling: The app processes JSON data returned by the API to extract relevant weather details. It also handles different units and stores search history.

Error Handling: Basic error handling is implemented to catch and display errors if the API request fails or the location is invalid.

Dynamic Background: The app changes its background color to reflect current weather conditions, providing a more immersive user experience.

Future Improvements
Enhanced Forecasting: Integrate real-time 8-day forecasts using the OpenWeatherMap API.

Customization Options: Allow users to customize the appearance of the app (e.g., theme, color scheme).

Advanced Error Handling: Improve error messages and handle specific cases like network issues or incorrect location input.

Mobile Compatibility: Extend the application to be compatible with mobile platforms.

Dependencies
OpenWeatherMap API: The app uses the OpenWeatherMap API to fetch weather data. Ensure you have a valid API key set in the WeatherAPI class.

