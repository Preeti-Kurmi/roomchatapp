# Secure Chat Room System

## Overview

This project is a robust chat room system built using JavaScript, Node.js, MySQL, and Express. The application ensures security, user authentication, and interactive communication. It includes features such as user registration and authentication, chat room creation, real-time messaging, profile viewing, and friend requests.

## Features

1. **User Registration and Authentication**
2. **Chat Room Creation**
3. **Inviting Participants**
4. **Joining a Room as a Non-Prime Member**
5. **Real-Time Chat Functionality**
6. **Profile Viewing**
7. **Friend Requests**
8. **Database Management**
9. **Security Measures**
10. **Error Handling and Validation**

## Getting Started

### Prerequisites

- Node.js (v14.x or higher)
- MySQL (v5.7 or higher)
- Git

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/Preeti-Kurmi/roomchatapp.git
    cd roomchatapp
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

3. Set up MySQL database:

    - Create a database named `chatroom`.
    - Run the provided SQL script to set up the database schema.
      ```sh
      mysql -u your_username -p chatroom < database/schema.sql
      ```

4. Configure environment variables:
    - Create a `.env` file in the root directory.
    - Add the following environment variables to the `.env` file:
      ```env
      PORT=3000
      DB_HOST=localhost
      DB_USER=your_username
      DB_PASSWORD=your_password
      DB_NAME=chatroom
      JWT_SECRET=your_jwt_secret
      ```

### Running the Application

1. Start the server:
    ```sh
    npm start
    ```

2. The application will be available at `http://localhost:3000`.

## API Endpoints

### User Registration and Authentication

- **Register a new user**
  ```http
  POST /api/register
