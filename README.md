# API-Testing-Portfolio

## Get synonyms for the word "sad"


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

![API Testing: Get word synonyms (wordsapi)](/assets/images/get-word-synonyms.png)













