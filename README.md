# 🌐 Node.js & MongoDB Social Media Dashboard

This is a full-stack backend application built with **Node.js** and **Express.js**, using **MongoDB** for data persistence. It features a complete user authentication system, post management (CRUD operations), and secure session handling.

## 🚀 Features

* **User Authentication**: Secure registration and login using **JSON Web Tokens (JWT)** and session-based storage.
* **CRUD Operations**: Users can create, read, update, and delete their own posts.
* **Request Validation**: Integrated logic to ensure data integrity before processing.
* **Security**: Implements practices like input sanitization and rate limiting to prevent common vulnerabilities.
* **Logging**: Comprehensive HTTP request and application-level logging.

## 🛠️ Tech Stack

* **Runtime**: Node.js
* **Framework**: Express.js
* **Database**: MongoDB with Mongoose ODM
* **Authentication**: JWT & Express-Session

## ⚙️ Installation & Setup

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/rnjhnd/node-mongodb-social-media-dashboard.git](https://github.com/rnjhnd/node-mongodb-social-media-dashboard.git)
    cd node-mongodb-social-media-dashboard
    ```
2.  **Install dependencies**:
    ```bash
    npm install
    ```
3.  **Set up Environment Variables**:
    Create a `.env` file and add your MongoDB connection string and JWT Secret:
    ```env
    PORT=3000
    MONGO_URI=mongodb://localhost:27017/SocialDB
    JWT_SECRET=your_secret_key
    ```
4.  **Run the application**:
    ```bash
    node app.js
    ```

## 📡 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **POST** | `/register` | Register a new user and redirect to dashboard |
| **POST** | `/login` | Authenticate user and start session |
| **GET** | `/posts` | Retrieve all posts for the logged-in user |
| **POST** | `/post` | Create a new post (Auth required) |
| **PUT** | `/posts/:id` | Update an existing post |
| **DELETE** | `/posts/:id` | Remove a post from the database |

## 🏛️ Architecture

The project follows the **MVC (Model-View-Controller)** pattern to ensure a clean separation of concerns, making the codebase easier to scale and maintain.

<img width="3999" height="1999" alt="image" src="https://github.com/user-attachments/assets/daa70028-08a0-424b-a4f9-e0cd37a2e1a4" />

