# API Automation Assignment

## Overview

This repository contains test strategy document, test scenarios document and automated tests for the [Reqres API](https://reqres.in/). The tests are designed to verify various functionalities of the API, including user registration, login, logout, user update, user delayed response, user creation, list all users, single user information and user deletion. The tests are implemented using Postman and cover both positive and negative scenarios.

## Prerequisites

Before running the tests, ensure you have the following installed:

- [Postman](https://www.postman.com/downloads/)

## Instructions

### 1. Import Postman Collection and Environment

1. **Download the Collection and Environment Files**
    - Download the `ReqRes API Tests.postman_collection` file containing the test cases.
    - Download the `ReqRes.postman_environment` file containing the necessary environment variables.

2. **Open Postman**
    - Launch the Postman application on your computer or Postman on the web, access the Postman API Platform through your web browser. Create a free account, and you're in.

3. **Import the Collection**
    - Click on the **Import** button in the top-left corner of Postman.
    - Select the `ReqRes API Tests.postman_collection` file and import it.

4. **Import the Environment**
    - Click on the **Environments** tab in the bottom-left corner of Postman.
    - Click on the **Import** button.
    - Select the `ReqRes.postman_environment` file and import it.

### 2. Set Up Environment Variables

The environment file contains necessary variables for the tests. Ensure the following variables are correctly set:

- 'baseUrl': Base URL for the Reqres API (default: 'https://reqres.in/api')
- 'userEmail': User email (default: 'eve.holt@reqres.in')
- 'userToken': User token (default: 'QpwL5tke4Pnpja7X4')
- 'userPassword': User password (default: 'cityslicka')

### 3. Run the Tests

1. **Select the Environment**
    - In the top-right corner of Postman, select the imported 'ReqRes' from the environment dropdown.

2. **Run Individual Requests**
    - Open the imported collection 'ReqRes API Tests'.
    - Click on any request to open it.
    - Click on the **Send** button to run the individual request and view the results.

3. **Run the Entire Collection**
    - Click on the **Collections** tab in the left sidebar.
    - Hover over the 'Reqres API Tests' collection and click on the **Run** button.
    - This will open the Collection Runner.
    - Ensure the correct environment ('Reqres') is selected.
    - Click on the **Start Run** button to execute all the tests in the collection.

### 4. Viewing Test Results

- After running the collection, the results will be displayed in the Collection Runner.
- You can view detailed logs for each request, including request/response data and test results.

## Test Scenarios Covered

### User Scenarios

1. **Register (Positive)**
    - Successful registration with valid data

2. **Register (Negative)**
    - Registration with missing required fields
  
3. **Login (Positive)**
    - Successful login with valid credentials

4. **Login (Negative)**
    - Login with invalid credentials
  
5. **Delayed Response**
    - Response received after a delay of 3 seconds.

6. **Logout**
    - Successful logout

### Admin Scenarios

1. **Update User**
    - Successful user update with valid data

2. **Delete User**
    - Successful user deletion
  
3. **User create**
    - The user is created successfully
  
4. **List Users**
    - Admin lists all users successfully

5. **Single User (Positive)**
    - Admin retrieves a single user successfully
  
6. **Single User (Negative)**
    - Admin tries to retrieve a non-existent user.

## Conclusion

By following the above instructions, you can import and run the automated tests for the Reqres API in Postman. These tests ensure the API functions correctly and handles various scenarios gracefully. Feel free to extend the tests and adapt them to cover additional cases as needed.

If you have any questions or need further assistance, please refer to the Postman [documentation](https://learning.postman.com/docs/getting-started/introduction/) or reach out to the repository maintainers.
