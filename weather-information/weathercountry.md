# weatherCountry()

#### `weatherCountry(country)`

Get weather information for a specific country.

* **Parameters:**
  * `country` (string): Name of the country.
* **Returns:**
  * Weather information including temperature, description, humidity, pressure, and wind speed.
*   **Example:**

    ```javascript
    const weatherData = await weatherCountry('Switzerland');
    if (weatherData) {
      weatherData.forEach(weather => {
        console.log("Temperature:", weather.temperature);
        console.log("Description:", weather.description);
        console.log("Humidity:", weather.humidity);
        console.log("Pressure:", weather.pressure);
        console.log("Wind Speed:", weather.windSpeed);
      });
    }
    ```
