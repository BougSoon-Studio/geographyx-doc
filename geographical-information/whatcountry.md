# whatCountry()

#### `whatCountry(field, value)`

Find a country based on a specific field value.

* **Parameters:**
  * `field` (string): Field to search.
  * `value` (string): Value to match.
* **Returns:**
  * One name a country matching the criteria.
*   **Example:**

    ```javascript
    const country = await whatCountry('continent', 'Europe');
    console.log(country);
    ```
