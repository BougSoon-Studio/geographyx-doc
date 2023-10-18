# Authentification

To use the GeographyX API, you need to authenticate with a valid user UID and token, available when you are logged in our website.

{% hint style="info" %}
You can obtain a token from the official website: [Get Token](https://blonality-studio.000.pe/api/get-token)
{% endhint %}

#### `Auth(userUID, token)`

Verify the authenticity of the user with the provided user UID and token.

* **Parameters:**
  * `userUID` (string): User UID.
  * `token` (string): Authentication token.
* **Returns:**
  * `true` if authentication is successful.
  * `false` if authentication fails.
*   **Example:**

    ```javascript
    const isAuthenticated = await Auth("MY-USER-UID", "MY-TOKEN");
    ```
