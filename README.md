
-# Social App API

This repository contains the backend API for a social networking application. The API is built with Node.js and Express, and it connects to a MongoDB database using Mongoose. It includes user authentication, post creation, and interaction features, making it a fully functional social media backend.

## Features

- **User Authentication**: JWT-based authentication with register and login functionality.
- **User Profiles**: Users can update their profiles and view other users' profiles.
- **Post Creation**: Users can create, edit, and delete posts.
- **Likes and Comments**: Users can like and comment on posts.
- **Follow System**: Allows users to follow and unfollow each other.

## Technologies Used

- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- bcrypt for password hashing

## Installation

1. Clone the repository:

    ```bash
  
    ```

2. Install the dependencies:

    ```bash
    npm install
    ```

3. Set up environment variables:

    Create a `.env` file in the root directory and add the following variables:

    ```bash
    MONGO_URI=your_mongo_uri
    JWT_SECRET=your_jwt_secret
    PORT=5000
    ```

4. Start the server:

    ```bash
    npm start
    ```

## API Endpoints

### Authentication

- `POST /api/auth/register`: Register a new user
- `POST /api/auth/login`: Log in a user

### Users

- `GET /api/users/:id`: Get a user's profile
- `PUT /api/users/:id`: Update a user's profile
- `DELETE /api/users/:id`: Delete a user's account
- `PUT /api/users/:id/follow`: Follow a user
- `PUT /api/users/:id/unfollow`: Unfollow a user

### Posts

- `POST /api/posts`: Create a new post
- `GET /api/posts/:id`: Get a specific post
- `PUT /api/posts/:id`: Update a post
- `DELETE /api/posts/:id`: Delete a post
- `PUT /api/posts/:id/like`: Like a post
- `POST /api/posts/:id/comment`: Comment on a post

## License

This project is open-source and available under the MIT License.

---

You can customize it further based on the specific functionalities you might want to emphasize or tweak. This template covers installation, setup, and core API features, providing a good starting point for the project documentation.
