# Example of the code

This is a example of a complet script :

```
<script type="module">
         import {
             Auth,
             getCountryInfo,
             fetchCountryData,
             getAllCountries,
             whatCountry,
             weatherCountry
         } from "https://blonality-studio.000.pe/geographyx/v2/geographyx.js";
        
         async function main() {
             try {
                 // Token verification
                 const MyToken = await Auth("USER_UID", "USER_TOKEN");
        
                 // Useful information for each country =>
                 const capital = await getCountryInfo('Switzerland', 'capital');
                 // Show in console
                 console.log(capital);
        
                 // All useful information for a country =>
                 const info = await getCountryInfo('Switzerland');
                 // Show in console
                 console.log(info);
        
                 // All countries =>
                 const allCountries = getAllCountries(await fetchCountryData());
                 // Show in console
                 console.log(allCountries);
        
                 // Country with a specific field value =>
                 const WhichCountryIsIt = await whatCountry('continent', 'Europe');
                 // Show in console
                 console.log(WhichCountryIsIt);

                 // Weather data for a country =>
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

             } catch (error) {
                 console.error(error.message);
             }
         }

         main();
     </script>
```
