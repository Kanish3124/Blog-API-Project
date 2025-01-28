# Blog Management System 📰

A full-stack application that allows users to create, view, edit, and delete blog posts. This project is divided into two servers: 
1. **API Server** - Handles all API requests for managing blog posts.
2. **Frontend Server** - Manages user interface and interaction.

---

## Features 🔗

- **View All Posts:** Fetch and display all blog posts.
- **Create Post:** Add a new blog post with a title, content, and author.
- **Edit Post:** Update any parameter of an existing blog post.
- **Delete Post:** Remove a blog post permanently.
- **Dynamic Routing:** Each post is accessible through its unique ID.

---

## Technologies Used 🚀

- **Backend:** Node.js, Express.js
- **Frontend:** EJS Templates
- **Database:** In-memory data store (for this implementation)
- **HTTP Client:** Axios

---

## Setup Instructions 🔧

### Prerequisites

- Node.js installed on your machine
- Basic knowledge of JavaScript and Express.js

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/blog-management-system.git
   cd blog-management-system
   ```

2. Install dependencies for both servers:

   ```bash
   cd api-server
   npm install
   cd ../frontend-server
   npm install
   ```

3. Start the API Server:

   ```bash
   cd api-server
   node index.js
   ```

   The API server will run on `http://localhost:4000`.

4. Start the Frontend Server:

   ```bash
   cd frontend-server
   node server.js
   ```

   The frontend server will run on `http://localhost:3000`.

---

## API Endpoints 🔀

### API Server (`http://localhost:4000`)

#### 1. Get All Posts
- **Endpoint:** `/posts`
- **Method:** GET
- **Response:** List of all posts.

#### 2. Get Post by ID
- **Endpoint:** `/posts/:id`
- **Method:** GET
- **Response:** Post with the specified ID.

#### 3. Create a New Post
- **Endpoint:** `/posts`
- **Method:** POST
- **Request Body:** JSON containing `title`, `content`, and `author`.
- **Response:** Created post.

#### 4. Update a Post (Partial)
- **Endpoint:** `/posts/:id`
- **Method:** PATCH
- **Request Body:** JSON containing any field to update (`title`, `content`, `author`).
- **Response:** Updated post.

#### 5. Delete a Post
- **Endpoint:** `/posts/:id`
- **Method:** DELETE
- **Response:** Confirmation message.

---

## Contributing 🛠️

Contributions are welcome! Feel free to submit a pull request or open an issue.

---

## Acknowledgements ✨

- [Express.js Documentation](https://expressjs.com/)
- [EJS Documentation](https://ejs.co/)
- [Axios Documentation](https://axios-http.com/)

---

## Author 💌
- Created by **Kanish**.  Happy Coding!
