# Product Inventory Management System (Backend)

A professional RESTful API built with Node.js and MongoDB to manage product inventories. This project features a robust CRUD system along with advanced functionality like searching, filtering, and pagination.

## 🚀 Key Features

* **Full CRUD Operations:** Create, Read, Update, and Delete products with ease.
* **Smart Search:** Search products by title using case-insensitive regular expressions.
* **Category Filtering:** Filter the product list based on specific categories.
* **Advanced Pagination:** Efficiently handle large datasets by loading data in chunks.
* **Data Validation:** Built-in Mongoose schema validation to ensure data integrity.
* **Environment Security:** Uses `.env` to keep sensitive database credentials secure.
* **Clean Architecture:** Organized folder structure following industry best practices.

## 🛠️ Tech Stack

* **Runtime:** Node.js
* **Framework:** Express.js
* **Database:** MongoDB (NoSQL)
* **ODM:** Mongoose
* **Config:** Dotenv

## 📁 Project Structure

```text
src/
├── config/          # Database connection configuration
├── controllers/     # Business logic & request handling
├── models/          # Mongoose Schemas & Data Models
├── routes/          # API Route definitions
├── .env             # Environment variables (Private)
├── app.js           # Application entry point
└── .gitignore       # Git exclusion rules
```

## ⚙️ Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone <your-repository-link>
   cd Product-Backend-NodeJS_and_MongoDB
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory and add:
   ```env
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/my_store
   ```

4. **Run the server:**
   ```bash
   node app.js
   # Or using nodemon
   nodemon app.js
   ```

## 📡 API Documentation

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **POST** | `/api/products` | Create a new product |
| **GET** | `/api/products` | Get all products (supports search, filter, paginate) |
| **GET** | `/api/products/:id` | Get details of a single product |
| **PUT** | `/api/products/:id` | Update an existing product |
| **DELETE** | `/api/products/:id` | Delete a product from the database |

### 🔍 Query Examples:

* **Search by Title:** `http://localhost:5000/api/products?title=laptop`
* **Filter by Category:** `http://localhost:5000/api/products?category=electronics`
* **Pagination:** `http://localhost:5000/api/products?page=1&limit=5`

---
**Developed by Muhammad Qasim**
```

---
