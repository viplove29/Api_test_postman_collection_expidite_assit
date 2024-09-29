# Postman API Testing - User and Ticket Management

# Overview

This project includes a Postman collection and environment for testing the User and Ticket Management API. The tests validate API functionality to ensure the correct creation of admin users, normal users, tickets, and cases. All tests target the API endpoint:
http://100.27.30.112/api/

Key API Tests:
# Admin User Creation
Verifies that admin users are created successfully.

# Normal User Creation
Ensures that normal users are created without issues.

# Ticket Creation and Verification
Tests the creation of a user ticket and verifies it using a GET request.

# Case Creation and Verification
Ensures that a case can be created and validated using a GET request.

# Setup Instructions

# Step 1:  Import Postman Collection and Environment

1. Download the Postman Collection
    Import the collection file provided in this repository into Postman. This file contains the API test requests for users, tickets, and cases.

2. Import the Postman Environment
    Import the environment file that includes the necessary variables such as base_url, admin_token, user_token, etc.

  To import:

  Open Postman.
  Navigate to File > Import.
  Upload both the collection and the environment file.
  
 ## Running the Tests
 
  1. Select the Environment
      Ensure that the correct environment is selected in the environment dropdown at the top-right corner of Postman.

2. Run the Collection

  Click on the Runner button in Postman.
  Choose the imported collection.
  Select the environment and click Start Run.

3. View Results
  Each test will validate the API responses for admin creation, normal user creation, and the creation and verification of tickets and cases.     You can check the results in the Test Results tab.

## Test Descriptions

Admin User Creation

POST request to /admin/users
Verifies if the admin user is successfully created and if the response status is 201.
Normal User Creation

POST request to /users
Verifies if a normal user is created successfully and checks for a status code of 201.
Ticket Creation and Verification

POST request to /tickets for ticket creation.
GET request to /tickets/{id} to verify the created ticket exists.
Case Creation and Verification

POST request to /cases for case creation.
GET request to /cases/{id} to verify the created case exists.


## Troubleshooting
  Ensure that the API base URL http://100.27.30.112/api/ is correct and accessible.
  Double-check that the environment variables are set properly, such as authentication tokens or user-specific details.
  Review API request headers and parameters to match the server expectations.
  Additional Notes
  The collection is designed to be flexible for various environments. Ensure the correct environment variables are in place before running the tests.
  You can view detailed API responses and logs within Postman’s Test Results and Console for troubleshooting.
  Enjoy testing your API!


This README covers the basic setup and usage of the Postman collection for API testing. Let me know if you need further modifications!

![image](https://github.com/user-attachments/assets/32f99027-8fcd-496c-bdd9-15361187217d)

![image](https://github.com/user-attachments/assets/fa7f546c-b68d-4c97-ab40-89c98f099a19)
