# Subscription Tracker

A **Node.js** and **Express**-based API for managing user subscriptions, authentication, and workflows. The application integrates **MongoDB** for data storage and supports secure user sessions using **JWT** and cookies. It is designed to support extensions with services like **Upstash** and **Arcjet**.

## Features

- ✅ User registration and authentication
- 📦 Subscription management
- 🔁 Workflow automation
- 🧩 API route versioning (`/api/v1`)
- 🗃️ MongoDB integration via Mongoose
- 🛡️ Middleware for security and error handling
- ⚙️ Environment-specific configuration support

## Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB with Mongoose
- **Authentication:** JWT, bcryptjs
- **Utilities:** dotenv, cookie-parser, morgan, nodemailer
- **Dev Tools:** ESLint, Nodemon

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) >= 18
- [npm](https://www.npmjs.com/)
- [MongoDB](https://www.mongodb.com/) instance (local or hosted)

### Installation

```bash
git clone https://github.com/yourusername/subscription-tracker.git
cd subscription-tracker
npm install
```

### Configuration

Create environment files (`.env.development.local`, `.env.production.local`) in the root directory with the following variables:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### Running the App

```bash
# Development
npm run dev

# Production
npm start
```

## API Endpoints

| Method | Endpoint                | Description            |
| ------ | ----------------------- | ---------------------- |
| GET    | `/api/v1/auth`          | Auth-related endpoints |
| GET    | `/api/v1/users`         | User-related endpoints |
| GET    | `/api/v1/subscriptions` | Manage subscriptions   |
| GET    | `/api/v1/workflows`     | Workflow integration   |

## Folder Structure

```text
.
├── app.js
├── config/
├── database/
├── middlewares/
├── routes/
├── controllers/
├── models/
└── utils/
```

## License

This project is licensed under the **MIT License**.

