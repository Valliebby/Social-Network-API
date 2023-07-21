# Social-Network-API

# This repository contains the code for a NoSQL-based Social Network API built using Express and Mongoose. This README provides instructions on how to use the API endpoints using Insomnia, a popular REST API client.

Table of Contents
Introduction
Features
Requirements
Getting Started
API Endpoints
Authentication
Error Handling
Contributing
License
Introduction
This API serves as the backend for a social networking platform built on a NoSQL database using MongoDB with Mongoose as the ODM (Object Data Modeling) library. It provides various endpoints for users to interact with the social network, such as creating and editing profiles, posting updates, following other users, and more.

Features
User registration and login
Create, read, update, and delete user profiles
Post, edit, and delete user updates
Follow and unfollow other users
Get the feed of followed users' updates
Requirements
Before running the API, make sure you have the following installed:

Node.js (https://nodejs.org/)
Insomnia REST Client
MongoDB (https://www.mongodb.com/)
Getting Started
Clone the repository and navigate to the project directory.

Install the dependencies using npm:
Copy code: git clone https://github.com/Valliebby/Social-Network-API.git
npm install
Rename the .env.example file to .env and set the environment variables according to your configuration. This file contains sensitive information such as the database connection URI.

Start the server:
Copy code: 
npm start
The API will be available at http://localhost:3001 by default. You can change the port by modifying the PORT environment variable in the .env file.

API Endpoints
The following are the available API endpoints:

POST /api/users/ - Create a new user
GET /api/users/:userId - Get the user's profile
PUT /api/users/:userId - Update the user's profile
POST /api/thoughts/:userId - Create a new post
PUT /api/users/:userId - Update a post by ID
DELETE /api/user/:id - Delete a user by ID
POST /api/users/:userId/friends/:userId - Follow a user by ID
DELETE /api/users/:userId/frinds/:userId - Unfollow a user by ID



https://github.com/Valliebby/Social-Network-API/assets/119483866/41f3638b-2ccc-43e8-8652-46199df767e8



Uploading SMN.mp4…


