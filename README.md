# Full-Stack CRUD Application

This is a full-stack CRUD (Create, Read, Update, Delete) application that includes both a backend and a frontend. The backend is built with Node.js, Express, and MongoDB, while the frontend is developed using React with Vite.

## Project Structure

- **client/**: Contains the frontend React application built with Vite.
- **server/**: Contains the backend Node.js/Express application.

## Features

- **Backend:**
  - Create a user
  - Retrieve all users or a specific user by ID
  - Update user information
  - Delete a user

- **Frontend:**
  - Forms for creating and updating users
  - Display list of all users

## Technologies Used

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB
  - Mongoose
  - CORS

- **Frontend:**
  - React.js
  - Vite
  - Axios (for making HTTP requests)

## Prerequisites

- **Node.js**: Ensure you have Node.js installed. You can download it from [nodejs.org](https://nodejs.org/).
- **MongoDB Atlas**: Create a MongoDB Atlas account and cluster, then configure the connection string.
- **React.js** and **Vite**: Basic knowledge of React and Vite is required to understand the frontend.

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/fullstack-crud-app.git
    cd fullstack-crud-app
    ```

2. **Install backend dependencies:**

    ```bash
    cd server
    npm install
    ```

3. **Install frontend dependencies:**

    ```bash
    cd ../client
    npm install
    ```

4. **Set up MongoDB connection:**

   Replace the MongoDB connection string in `server/server.js` with your own connection string:
   
    ```javascript
    mongoose.connect("mongodb+srv://<username>:<password>@cluster0.mongodb.net/Crud?retryWrites=true&w=majority");
    ```

5. **Run the backend server:**

    ```bash
    cd ../server
    npm start
    ```

    The server will start on `http://localhost:3001`.

6. **Run the frontend:**

    ```bash
    cd ../client
    npm run dev
    ```

    The React application will start on `http://localhost:3000`.

## API Endpoints (Backend)

- **GET /:**  
  Retrieves all users.

- **GET /getUser/:id:**  
  Retrieves a specific user by their ID.

- **POST /createUser:**  
  Creates a new user with the provided data.

- **PUT /updateUser/:id:**  
  Updates the user with the specified ID.

- **DELETE /deleteUser/:id:**  
  Deletes the user with the specified ID.
