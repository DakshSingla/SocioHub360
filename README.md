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
frontend/  React application
backend/   Express API and database models
```
