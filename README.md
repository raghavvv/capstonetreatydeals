# TreatyDeals

TreatyDeals is a full-stack MERN (MongoDB, Express, React, Node.js) web application for booking home services at the best prices and discounts. Users can browse, book, and manage services provided by local vendors, while vendors (managers) can register their shops and manage their offerings.

## Features

- **User Authentication:** Register and log in as a user or service provider (manager).
- **Role-based Access:** Users can book services; managers can create and manage their own shops and services.
- **Service Browsing:** View all available services and detailed information about each.
- **Order Management:** Users can place orders for services and track their status.
- **Manager Dashboard:** Managers can add new shops, define services (meals), and view orders.
- **Responsive UI:** Built with React and Materialize CSS for a modern, responsive interface.

## Tech Stack

- **Frontend:** React, Redux, Axios, Materialize CSS
- **Backend:** Node.js, Express.js, MongoDB (Mongoose)
- **Authentication:** JWT (JSON Web Tokens), Passport.js
- **State Management:** Redux, Redux Thunk
- **Testing:** Mocha, Should, Supertest

## Folder Structure

```
.
├── client/                 # React frontend
│   ├── src/
│   │   ├── actions/
│   │   ├── components/
│   │   ├── reducers/
│   │   ├── utils/
│   │   ├── App.js
│   │   └── ...
│   └── public/
├── routes/                 # Express API routes
│   ├── api/
│   │   ├── auth/
│   │   ├── meal/
│   │   ├── order/
│   │   ├── restaurant/
│   │   └── user/
├── config/                 # Configuration files (keys, passport)
├── validation/             # Input validation logic
├── server.js               # Express server entry point
└── package.json            # Project dependencies and scripts
```

## Getting Started

### Prerequisites

- Node.js (v12+)
- npm
- MongoDB Atlas account (or local MongoDB)

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/treatydeals.git
   cd treatydeals
   ```

2. **Install server dependencies:**
   ```sh
   npm install
   ```

3. **Install client dependencies:**
   ```sh
   npm run client-install
   ```

4. **Set up environment variables:**
   - Edit `config/keys.js` with your MongoDB URI and JWT secret.

5. **Run the application (development mode):**
   ```sh
   npm run dev
   ```
   - This will start both the backend server and the React client.

6. **Run tests:**
   ```sh
   npm test
   ```

## Usage

- Visit `http://localhost:3000` to access the frontend.
- Register as a user or manager.
- Managers can create shops and add services.
- Users can browse services, place orders, and track their status.

## Scripts

- `npm run dev` - Run both server and client in development mode
- `npm start` - Run only the server
- `npm run client` - Run only the React client
- `npm test` - Run backend tests
