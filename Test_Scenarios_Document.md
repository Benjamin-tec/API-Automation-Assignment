## Test Scenarios

### User

1. **Register - Positive**
   - **Scenario**: Successful user registration with valid details.
   - **Given**: A new user with valid registration details.
   - **When**: The user submits the registration form.
   - **Then**: The user is registered successfully, and a confirmation message is returned.

2. **Register - Negative**
   - **Scenario**: User registration with missing or invalid details.
   - **Given**: A new user with missing or invalid registration details.
   - **When**: The user submits the registration form.
   - **Then**: An error message is returned, indicating the issue.

3. **Login - Positive**
   - **Scenario**: Successful user login with valid credentials.
   - **Given**: An existing user with valid credentials.
   - **When**: The user submits the login form.
   - **Then**: The user is logged in successfully, and a token is returned.

4. **Login - Negative**
   - **Scenario**: User login with invalid credentials.
   - **Given**: A user with invalid credentials.
   - **When**: The user submits the login form.
   - **Then**: An error message is returned, indicating invalid credentials.

5. **Logout**
   - **Scenario**: Successful user logout.
   - **Given**: A logged-in user.
   - **When**: The user requests to log out.
   - **Then**: The user is logged out successfully, and a confirmation message is returned.

### Admin

1. **Update User - Positive**
   - **Scenario**: Admin updates a user's details with valid data.
   - **Given**: An admin with valid credentials and a user to update.
   - **When**: The admin submits valid update details.
   - **Then**: The user's details are updated successfully, and a confirmation message is returned.

2. **Update User - Negative**
   - **Scenario**: Admin updates a user's details with invalid data.
   - **Given**: An admin with valid credentials and a user to update.
   - **When**: The admin submits invalid update details.
   - **Then**: An error message is returned, indicating the issue.

3. **Delete User - Positive**
   - **Scenario**: Admin deletes a user successfully.
   - **Given**: An admin with valid credentials and a user to delete.
   - **When**: The admin requests to delete the user.
   - **Then**: The user is deleted successfully, and a confirmation message is returned.

4. **Delete User - Negative**
   - **Scenario**: Admin tries to delete a non-existent user.
   - **Given**: An admin with valid credentials and a non-existent user ID.
   - **When**: The admin requests to delete the non-existent user.
   - **Then**: An error message is returned, indicating the user does not exist.

5. **View User Details - Positive**
   - **Scenario**: Admin views a user's details successfully.
   - **Given**: An admin with valid credentials and a user to view.
   - **When**: The admin requests to view the user's details.
   - **Then**: The user's details are returned successfully.
