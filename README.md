# API-Testing-Portfolio

## Get synonyms for the word "sad" on https://www.wordsapi.com/ 


### Project Overview

This project contains automated tests for the WordsAPI /words/{word}/synonyms endpoint, which returns synonyms for a given word.


### Tested Endpoint

GET https://wordsapiv1.p.rapidapi.com/words/sad/synonyms 

Example tested with the word: sad 


### Request Details

Method: GET 

URL: https://wordsapiv1.p.rapidapi.com/words/sad/synonyms 

Headers:

  - x-rapidapi-host: wordsapiv1.p.rapidapi.com
  - x-rapidapi-key: Your API Key (353b4bad4emsh18da20418167ddbp1154adjsn57bf237f2a94)


### Project Structure

  - **API Test in Postman:** The test is configured in Postman and can be run directly from the application.
  - **The purpose of this test is to verify:**
          - The API returns a successful HTTP status code (200 OK);
          - The response contains the expected word property with the correct value;
          - The response contains a non-empty array of synonyms;
          - Each synonym in the array is a string.
    

### Steps to run the test

  1. In Postman, insert the Endpoint.
  2. Add required headers (x-rapidapi-key, x-rapidapi-host).
  3. Click on the "Send" button to execute the test.
  4. Review the results in Postman’s console to determine which tests were successful and which failed.

### Test Details

1. Response Status Code: Verifies that the API returns a 200 / Success status code, indicating the request was successful.

2. Word Property: Ensures that the response contains the property "word" with the correct value (e.g., "sad").

3. Synonyms Array Exists: Confirms that the API returns a non-empty array of synonyms.

4. Synonyms Data Type: Checks that each item in the synonyms array is a string, ensuring data consistency.


### Test Results

  - If all tests pass successfully, the API correctly returns a valid list of synonyms for the requested word.
  - Postman will indicate any failed tests and provide information to help identify the issue.


### Example

![API Testing: Get word synonyms (wordsapi)](images/get-word-synonyms.png)


---


## API Test: Get current weather by city name using [api.openweathermap.org ](https://openweathermap.org/api) 

### Project Overview 

This project contains automated tests for the OpenWeatherMap /data/2.5/weather endpoint, which returns the current weather data for a specific city.

The purpose of this test is to verify:

- That the API returns a successful response (status code 200);
- That the city name in the response matches the requested city;
- That essential weather-related properties are present in the response (e.g., temperature, humidity, weather description);
- That values are in expected formats and units (e.g., temperature in Celsius, language in Romanian).

### Tested Endpoint

GET [https://api.openweathermap.org/data/2.5/weather](https://api.openweathermap.org/data/2.5/weather) 

### Parameters

- q: city name; in this case: 'London'
- appid: unique API key
- (Optional) mode: defines the response format; Accepted values are xml and html. If this parameter is not specified, the       API defaults to returning the response in JSON format. 
- (Optional) units: units of measurement;
  
  Temperature is available in Fahrenheit, Celsius and Kelvin units.

    - For temperature in Fahrenheit use units=imperial;
    - For temperature in Celsius use units=metric;
  
    *Temperature in Kelvin is used by default, no need to use units parameter in API call.

- (Optional) lang: specifies the desired language for the response; Translation is applied to selected fields, including the city name and weather description.












