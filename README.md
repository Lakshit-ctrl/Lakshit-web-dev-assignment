# Lakshit - Web Dev Assignment

A RESTful backend application built using **Node.js, Express.js, MongoDB and Mongoose**.

This project demonstrates user registration, login and CRUD (Create, Read, Update, Delete) operations through REST APIs.

## Author

- **Name:** Lakshit
- **Email:** lakshitprajapat2008@gmail.com
- **GitHub:** [@lakshit-ctrl](https://github.com/lakshit-ctrl)

## Technologies Used

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JavaScript
- Postman / REST Client
- Git and GitHub

## Project Structure

```text
lakshit-web-dev-assignment/
├── backend/
│   └── src/
│       ├── config/
│       ├── controllers/
│       ├── models/
│       ├── routes/
│       └── index.js
├── postman/
│   └── Lakshit_Web_Dev_Assignment.postman_collection.json
├── requests.http
├── .env.example
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

## Installation and Setup

### 1. Clone or open the repository

```bash
git clone https://github.com/lakshit-ctrl/lakshit-web-dev-assignment.git
cd lakshit-web-dev-assignment
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root.

Add the following configuration:

```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string/lakshit-web-dev-assignment
```

Replace the MongoDB URI placeholder with your own Atlas connection string or local MongoDB URI.

**Never upload your `.env` file or database credentials to GitHub.**

### 4. Start the server

```bash
npm run dev
```

The server runs on the configured port (`http://localhost:4000`).

## API Endpoints

Base URL:

```text
http://localhost:4000
```

### User APIs

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/v1/users/register` | Register a user |
| POST | `/api/v1/users/login` | Login a user |
| POST | `/api/v1/users/logout` | Logout endpoint |

### Post APIs

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/v1/posts/create` | Create a post |
| GET | `/api/v1/posts/getPosts` | Retrieve all posts |
| PATCH | `/api/v1/posts/update/:id` | Update a post |
| DELETE | `/api/v1/posts/delete/:id` | Delete a post |

## Post Data Format

Example JSON request:

```json
{
  "name": "Lakshit",
  "description": "My first backend project post",
  "age": 18
}
```

## Testing

The APIs can be tested using the included `requests.http` (REST Client) or Postman.

Test requests are provided for:

- User Registration
- User Login
- User Logout
- Create Post
- Get All Posts
- Update Post
- Delete Post

## Learning Reference

This project was developed as an academic backend assignment by Lakshit, using the backend development tutorial ([Intro to Backend Web Development – Node.js & Express](https://www.youtube.com/watch?v=KOutPbKc9UM)) as a learning reference. The implementation was configured, tested, and customized for this assignment.

## License

This project is intended for academic and educational purposes.
