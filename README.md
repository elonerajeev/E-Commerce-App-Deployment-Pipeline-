
# Full-Stack E-Commerce MERN App

A comprehensive e-commerce application using the MERN stack (MongoDB, Express.js, React.js, Node.js). This project allows for managing products, categories, and user interactions in an online store.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Setup](#setup)
- [Features](#features)
- [API Reference](#api-reference)
- [Acknowledgements](#acknowledgements)
- [Authors](#authors)
- [License](#license)

## Project Overview

This project demonstrates a modern e-commerce platform using the MERN stack. It consists of:

- **Frontend**: Built with React.js to handle the user interface and interactions.
- **Backend**: Built with Node.js and Express.js to manage API requests, database interactions, and authentication.

## Installation

To get started with the Full-Stack E-Commerce MERN App, follow these steps:

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [npm](https://www.npmjs.com/) (v6 or higher) or [Yarn](https://yarnpkg.com/) (optional)
- [MongoDB](https://www.mongodb.com/try/download/community) (or use MongoDB Atlas for cloud deployment)

### Backend Installation

1. **Navigate to the Backend Directory:**

   ```bash
   cd backend
   ```

2. **Install Backend Dependencies:**

   ```bash
   npm install
   ```

3. **Set Up Environment Variables:**

   - Create a `.env` file in the `backend` directory.
   - Add the following environment variables:

     ```plaintext
     MONGO_URI=<Your MongoDB Connection String>
     PORT=5000
     FRONTEND_URL=<Your Frontend URL>
     JWT_SECRET=<Your JWT Secret>
     ```

4. **Run Backend Server:**

   ```bash
   npm start dev
   ```

### Frontend Installation

1. **Navigate to the Frontend Directory:**

   ```bash
   cd frontend
   ```

2. **Install Frontend Dependencies:**

   ```bash
   npm install
   ```

3. **Run Frontend Development Server:**

   ```bash
   npm start
   ```

The frontend will be accessible at `http://localhost:3000` and the backend at `http://localhost:8080` by default. Ensure both servers are running to fully interact with the application.

### Optional: Running Tests

- **For Backend:**

  ```bash
  cd backend
  npm test
  ```

- **For Frontend:**

  ```bash
  cd frontend
  npm test
  ```

### Troubleshooting

- Ensure all environment variables are correctly set and that both backend and frontend servers are running without errors.
- Check the console for error messages and consult documentation or issue trackers for help.

## Setup

### Project Structure

The project is organized into two main directories:

1. **`frontend`**: Contains the React.js application for the user interface.
2. **`backend`**: Contains the Node.js and Express.js application for server-side logic and API endpoints.

### File Structure

**Frontend:**
- `src/`: Contains the main React application code.
- `public/`: Static assets and HTML file.

**Backend:**
- `src/`: Contains the server-side code, including routes, controllers, and models.
- `.env`: Environment variables for configuration.
- `config/`: Configuration files for the database and other services.

## Features

- **Product Management**: Add, update, and delete products.
- **Category Management**: Organize products into categories.
- **User Authentication**: Register, log in, and manage user sessions.
- **Cart Functionality**: Add products to the shopping cart and proceed to checkout.
- **Order Processing**: Place orders and view order history.

## API Reference

| Endpoint                 | Method | Description                       |
|--------------------------|--------|-----------------------------------|
| `/api/products`          | GET    | Get all products                  |
| `/api/products/:id`      | GET    | Get a single product by ID         |
| `/api/products`          | POST   | Add a new product                  |
| `/api/products/:id`      | PUT    | Update a product by ID             |
| `/api/products/:id`      | DELETE | Delete a product by ID             |
| `/api/categories`        | GET    | Get all categories                 |
| `/api/categories/:id`    | GET    | Get a single category by ID         |
| `/api/categories`        | POST   | Add a new category                 |
| `/api/categories/:id`    | PUT    | Update a category by ID            |
| `/api/categories/:id`    | DELETE | Delete a category by ID            |
| `/api/users/register`    | POST   | Register a new user                |
| `/api/users/login`       | POST   | Log in a user                      |
| `/api/cart`              | GET    | Get user's cart                    |
| `/api/cart/add`          | POST   | Add an item to the cart            |
| `/api/cart/remove`       | POST   | Remove an item from the cart       |
| `/api/orders`            | POST   | Place an order                     |
| `/api/orders/:id`        | GET    | Get order details by ID            |

## Acknowledgements

- [MERN Stack Documentation](https://www.mongodb.com/mern-stack)
- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [Node.js Documentation](https://nodejs.org/en/docs/)
- [Express.js Documentation](https://expressjs.com/)


## Authors

- **Rajeev Kumar**: [LinkedIn](https://www.linkedin.com/in/rajeev-kumar-2209b1243) | [GitHub](https://github.com/elonerajeev)
- **Elone Rajeev**: [LinkedIn](https://www.linkedin.com/in/rajeev-kumar-2209b1243) | [GitHub](https://github.com/elonerajeev)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

