# getCountryInfo()

#### `getCountryInfo(country, field)`

Get specific information about a country.

* **Parameters:**
  * `country` (string): Name of the country.
  * `field` (string, optional): Specific field to retrieve.
* **Returns:**
  * Information about the country.
*   **Example:**

    ```javascript
    const capital = await getCountryInfo('Switzerland', 'capital');
    console.log(capital);

    const infos = await getCountryInfo('Switzerland');
    console.log(infos);
    ```
