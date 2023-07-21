# Social-Network-API

# This repository contains the code for a NoSQL-based Social Network API built using Express and Mongoose. This README provides instructions on how to use the API endpoints using Insomnia, a popular REST API client.

Table of Contents
Introduction
Requirements
Getting Started
API Endpoints
Authentication
Error Handling
Contributing
License
Introduction
This API serves as the backend for a social networking platform built on a NoSQL database using MongoDB with Mongoose as the ODM (Object Data Modeling) library. It provides various endpoints for users to interact with the social network, such as creating and editing profiles, posting updates, following other users, and more.

Requirements
Before using the API in Insomnia, make sure you have the following installed:

Insomnia REST Client
Getting Started
Clone the repository and navigate to the project directory.

Install the dependencies using npm:

bash
Copy code
npm install
Rename the .env.example file to .env and set the environment variables according to your configuration. This file contains sensitive information such as the database connection URI and JWT secret, so keep it secure and never commit it to version control.

Start the server:

bash
Copy code
npm start
The API will be available at http://localhost:3000 by default. You can change the port by modifying the PORT environment variable in the .env file.

API Endpoints
The following are the available API endpoints:

Register a new user

URL: POST /api/users/register
Parameters:
name (string): User's name
email (string): User's email address
password (string): User's password
Response: The response will contain the newly registered user's information.
User login

URL: POST /api/users/login
Parameters:
email (string): User's email address
password (string): User's password
Response: Upon successful login, the response will contain a JWT token that should be used for authentication in subsequent requests.
Get the user's profile

