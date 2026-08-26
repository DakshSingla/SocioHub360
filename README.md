# SocioHub360

SocioHub360 is a full-stack web application for managing a residential society. It provides a simple dashboard for residents and administrators to manage visitors, maintenance requests, announcements, amenities, and payments.

## Tech used

- React and Tailwind CSS for the frontend
- Node.js and Express for the backend
- MongoDB for the database

## Run locally

1. Install Node.js and MongoDB.
2. Install dependencies:

```bash
npm run install-all
```

3. Create `backend/.env` from `backend/.env.example` and set your MongoDB connection string and JWT secrets.
4. Start the project:

```bash
npm run dev
```

The frontend runs on `http://localhost:3000` and the backend runs on `http://localhost:5000`.

## Main features

- User registration and login
- Visitor management
- Maintenance and complaint tracking
- Announcements and notifications
- Amenities and payment management

## Project structure

```text
SocioHub360/
├── frontend/                 React application
│   ├── public/               Images, icons, and public files
│   └── src/
│       ├── components/       Pages and reusable UI components
│       ├── contexts/         Shared application state
│       ├── services/         API request functions
│       ├── App.js            Main frontend component
│       └── index.js          Frontend entry point
│
├── backend/                  Node.js and Express server
│   ├── src/
│   │   ├── config/           Database configuration
│   │   ├── middleware/       Authentication and validation middleware
│   │   ├── models/           MongoDB models
│   │   ├── routes/           API route files
│   │   └── server.js         Backend entry point
│   └── .env.example          Environment variable template
│
├── package.json              Root scripts and dependencies
└── README.md                 Project information
```

## Features

- Register and log in as a user
- Manage society visitors and their entry details
- Raise and track maintenance or complaint requests
- View announcements and notifications
- Manage amenities, payments, and finance-related details
- Use an admin dashboard for basic society management

## Prerequisites

Install the following before running the project:

- Node.js (version 16 or later)
- npm
- MongoDB, either local MongoDB or MongoDB Atlas

## Installation and setup

Clone the repository and open the project folder:

```bash
git clone https://github.com/DakshSingla/SocioHub360.git
cd SocioHub360
```

Install all project dependencies:

```bash
npm run install-all
```

Create a local backend environment file by copying `backend/.env.example` to `backend/.env`. At minimum, update these values:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/society360
JWT_SECRET=add_a_long_random_secret
JWT_REFRESH_SECRET=add_another_long_random_secret
FRONTEND_URL=http://localhost:3000
```

Do not commit `backend/.env` because it may contain private keys or database credentials.

## Available commands

Run these commands from the project root:

| Command | Description |
| --- | --- |
| `npm run install-all` | Installs root, backend, and frontend dependencies. |
| `npm run dev` | Starts the backend and frontend together for development. |
| `npm run server` | Starts only the backend development server. |
| `npm run client` | Starts only the React frontend. |
| `npm run build` | Creates a production build of the frontend. |
| `npm start` | Starts the backend in production mode. |

## Running the project

Start MongoDB first, then run:

```bash
npm run dev
```

Open `http://localhost:3000` in a browser. The frontend communicates with the API at `http://localhost:5000`.

## API modules

The backend is organised into route modules for authentication, users, visitors, maintenance, amenities, communication, administration, finance, and payments. API requests are handled by the frontend through `frontend/src/services/api.js`.

## Author

Daksh Singla
