## Test Scenarios

### User

1. **Register - Positive**
   - **Scenario**: Successful user registration with valid details.
   - **Given**: The user provides valid registration data.
   - **When**: The user sends a POST request to the /register endpoint.
   - **Then**: The user is registered successfully.

2. **Register - Negative**
   - **Scenario**: User registration with missing or invalid details.
   - **Given**: The user provides incomplete registration data.
   - **When**: The user sends a POST request to the /register endpoint.
   - **Then**: An error message is returned, indicating the issue.

3. **Login - Positive**
   - **Scenario**: Successful user login with valid credentials.
   - **Given**: An existing user with valid credentials.
   - **When**: The user sends a POST request to the /login endpoint.
   - **Then**: The user is logged in successfully, and a token is returned.

4. **Login - Negative**
   - **Scenario**: User login with invalid credentials.
   - **Given**: A user with invalid credentials.
   - **When**: The user sends a POST request to the /login endpoint.
   - **Then**: An error message is returned, indicating invalid credentials.

5. **Delayed Response**
   - **Scenario**: User experiences a delayed response.
   - **Given**: The user sent request after a delay of 3 seconds.
   - **When**: The response should be delayed.
   - **Then**: Response received after a delay of 3 seconds.

6. **Logout**
   - **Scenario**: Successful user logout.
   - **Given**: A logged-in user.
   - **When**: The user sends a POST request to the /logout endpoint.
   - **Then**: The user is logged out successfully, and a confirmation message is returned.

### Admin

1. **Update User - Positive**
   - **Scenario**: Admin updates a user's details with valid data.
   - **Given**: An admin with valid credentials and a user to update.
   - **When**: The admin sends a PUT request to the /users/{id} endpoint.
   - **Then**: The user's details are updated successfully, and a confirmation message is returned.

2. **Update User - Negative**
   - **Scenario**: Admin updates a user's details with invalid data.
   - **Given**: An admin with valid credentials and a user to update.
   - **When**: The admin sends a PUT request to the /users/{id} endpoint.
   - **Then**: An error message is returned, indicating the issue.

3. **Delete User - Positive**
   - **Scenario**: Admin deletes a user successfully.
   - **Given**: An admin with valid credentials and a user to delete.
   - **When**: The admin sends a DELETE request to the /users/{id} endpoint.
   - **Then**: The user is deleted successfully, and a confirmation message is returned.
  
4. **Create User (Positive)**
   - **Scenario**: Admin creates a new user successfully
   - **Given**: An admin provide valid details to create a new user
   - **When**: The admin sends a POST request with new user data to the /users/{id} endpoint.
   - **Then**: The user is created successfully, the system should return the new user's details.

5. **List Users - Positive**
   - **Scenario**: Admin lists all users successfully.
   - **Given**: An admin with valid credentials.
   - **When**: The admin sends a GET request to the /users?page=2 endpoint.
   - **Then**: The list of users is returned successfully.

6. **Single User - Positive**
   - **Scenario**: Admin retrieves a single user successfully.
   - **Given**: An admin with valid credentials and a valid user ID.
   - **When**: The admin sends a GET request to the /users/{id} endpoint.
   - **Then**: The user's details are returned successfully.
  
7. **Single User - Negative**
   - **Scenario**: Admin tries to retrieve a non-existent user.
   - **Given**: An admin with valid credentials and a non-existent user ID.
   - **When**: The admin sends a GET request to the /users/{id} endpoint.
   - **Then**: An error message is returned, indicating the user does not exist.
