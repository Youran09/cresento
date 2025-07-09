# Cresento Backend API

Backend API for the Cresento AI Shin Guards website.

## Features

- User authentication (register, login, profile)
- Newsletter subscription
- Contact form submission
- SQLite database for data storage
- JWT token-based authentication
- CORS enabled for frontend integration

## Installation

1. Navigate to the backend directory:
   ```bash
   cd cresento-backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Update the `.env` file with your configuration:
   ```
   PORT=5000
   JWT_SECRET=your-super-secret-jwt-key
   NODE_ENV=development
   ```

4. Start the server:
   ```bash
   npm run dev
   ```

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/profile` - Get user profile (requires authentication)

### Newsletter
- `POST /api/newsletter/subscribe` - Subscribe to newsletter

### Contact
- `POST /api/contact` - Submit contact form

### Admin
- `GET /api/admin/subscribers` - Get all newsletter subscribers
- `GET /api/admin/contacts` - Get all contact submissions

### Health
- `GET /api/health` - Health check endpoint

## Database Schema

The API uses SQLite with the following tables:

- `users` - User accounts
- `newsletter_subscribers` - Newsletter subscriptions
- `contact_submissions` - Contact form submissions

## Security

- Passwords are hashed using bcrypt
- JWT tokens are used for authentication
- CORS is configured for frontend integration
- Input validation on all endpoints