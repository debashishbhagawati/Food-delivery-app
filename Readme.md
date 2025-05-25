# Deliva

A full-stack web application for seamless online food ordering, built with JavaScript (React + Express), with separate admin and user frontends and a robust backend using MongoDB.

---

## Features

- **User Panel**
  - Browse food menu and categories
  - Add items to cart and manage orders
  - User authentication and profile management
  - Secure checkout with Stripe integration

- **Admin Panel**
  - Manage menu items (CRUD)
  - Manage orders and users
  - View sales analytics

- **Backend**
  - RESTful API with Express.js
  - MongoDB database (Mongoose ODM)
  - JWT authentication
  - File uploads for food images

---

## Tech Stack

- **Front-end:** React, Vite, React Router, Axios
- **Admin Panel:** React, Vite, React-Toastify
- **Back-end:** Node.js, Express.js, MongoDB, Mongoose, Stripe
- **Other:** Multer (file uploads), JWT (authentication), dotenv

---

## Folder Structure

```
Food-delivery-app/
│
├── admin/        # Admin dashboard (React + Vite)
├── front-end/    # User-facing app (React + Vite)
├── back-end/     # Express server, API, MongoDB models
```

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm or yarn
- MongoDB database (local or Atlas)

### 1. Clone the repository

```bash
git clone https://github.com/debashishbhagawati/Food-delivery-app.git
cd Food-delivery-app
```

### 2. Install dependencies

```bash
# Install backend dependencies
cd back-end
npm install

# Install frontend dependencies
cd ../front-end
npm install

# Install admin dependencies
cd ../admin
npm install
```

### 3. Set up environment variables

- Create a `.env` file in `/back-end` with the following:
  ```
  PORT=4000
  MONGODB_URI=your_mongodb_connection_string
  JWT_SECRET=your_jwt_secret
  STRIPE_SECRET_KEY=your_stripe_secret_key
  ```
- Update the connection string in `server.js` if needed.

### 4. Run the servers

- **Backend:**
  ```bash
  cd back-end
  npm start
  ```
- **Frontend (User):**
  ```bash
  cd ../front-end
  npm run dev
  ```
- **Admin Panel:**
  ```bash
  cd ../admin
  npm run dev
  ```

---

## API Endpoints (Backend)

- `/api/food` — Food items & categories
- `/api/user` — User auth & profile
- `/api/cart` — Cart management
- `/api/order` — Order management
- `/images` — Uploaded images

---

## License

MIT

---

## Author

[Debashish Bhagawati](https://github.com/debashishbhagawati)
