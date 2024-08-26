**Name:** AKASH KUMAR  
**Company:** CODTECH IT SOLUTIONS  
**ID:** CT04DS6313  
**Domain:** Backend  
**Duration:** August to September 2024  
**Mentor:** Muzammil Ahmed  

# Basic Authentication System

## *Overview of the Project*

### *Project*: *Basic Authentication System*

### *Objective*  
The objective of this project is to implement a basic authentication system with registration and login functionality. The system uses Node.js with Express.js for the backend and MongoDB for storing user credentials securely. It includes user registration, login, and token-based authentication.

### *Key Activities*  
- **User Registration**: *Allowing users to create accounts with a username and password.*
- **User Login**: *Authenticating users with stored credentials and generating a token upon successful login.*
- **Data Storage**: *Storing user credentials securely in MongoDB using bcrypt for password hashing.*
- **Token-Based Authentication**: *Using JSON Web Tokens (JWT) to manage user sessions.*

### *Technologies Used*  
- **Node.js**: *JavaScript runtime for server-side development.*
- **Express.js**: *Web framework for building the REST API.*
- **MongoDB**: *NoSQL database for storing user data.*
- **bcrypt**: *Library for hashing passwords securely.*
- **jsonwebtoken**: *Library for creating and verifying JSON Web Tokens (JWT).*
- **HTML/CSS**: *For creating and styling the login and registration pages.*

## *Installation*

1. **Install Dependencies**:
   npm install
   
2. **Start MongoDB**:
   mongod

3. **Start the Server**:
   npm start

 The server will start on http://localhost:3000.
## *API Endpoints*

- **POST /api/auth/register**
  - **Description**: Registers a new user with a username and password.
  - **Request Body**:
    ```json
    {
      "username": "exampleUser",
      "password": "examplePassword"
    }
    ```
  - **Response**: JSON object with a success message.
  - **Register.html page**
  - ![357785993-89fb11e8-46f2-4896-bbcf-f190f1dc00f5](https://github.com/user-attachments/assets/24c8e8cc-15a1-4884-99c9-7f9996871e8a)
  - ![Screenshot 2024-08-26 201551](https://github.com/user-attachments/assets/adc1b728-7f3b-4486-9318-ecdc07cb8cd6)



- **POST /api/auth/login**
  - **Description**: Authenticates a user and returns a JWT token.
  - **Request Body**:
    ```json
    {
      "username": "exampleUser",
      "password": "examplePassword"
    }
    ```
  - **Response**: JSON object with a token:
    ```json
    {
      "token": "your-jwt-token"
    }
    ```
 - **login.html**
 - ![Screenshot 2024-08-26 201458](https://github.com/user-attachments/assets/3386eb71-5c85-429f-b9cb-034d63904b4c)
 - ![Screenshot 2024-08-26 201627](https://github.com/user-attachments/assets/318e22ad-fc13-4c84-8950-761b616a50d5)
- **Mongodb compass output**
- The user information is stored on the mongodb database.
-  ![357787050-c8ef3cbd-6bb7-49de-b349-06e947e30606](https://github.com/user-attachments/assets/51b3fe63-e913-4fdd-b5f6-fbbb410cfd94)


## *Project Structure*

- **public/**
  - **login.html**: HTML file for the login page.
  - **register.html**: HTML file for the registration page.

- **src/**
  - **app.js**: Main server file with routes and server configuration.
  - **authRoutes.js**: Defines authentication-related routes.
  - **userModel.js**: Defines the user schema and model for MongoDB.


