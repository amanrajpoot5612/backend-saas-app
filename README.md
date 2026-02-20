# CORE TECH STACK

- Node.js
- Express
- MongoDB (or Postgres)
- JWT authentication
- Environment config
- Basic logging

# Packages and libraries used:

- express
- mongoose
- jsonwebtoken
- bcrypt
- dotenv
- cors
- helmet
- morgan
- zod (for validation)

# Project Structure

```
src/
 ├── config/
 ├── modules/
 │    ├── auth/
 │    ├── user/
 │    ├── assessment/
 │    ├── submission/
 │    └── interview/
 ├── middleware/
 ├── utils/
 ├── services/
 ├── routes/
 ├── app.js
 └── server.js
 ```

# Setup Instructions

1. Clone the repository
2. Install dependencies: `npm install`
3. Create a `.env` file based on `.env.example`
4. Start the server: `npm start`
5. Run tests: `npm test`

# API Endpoints
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login and receive a JWT
- `GET /api/user/profile` - Get user profile (protected)
- `POST /api/assessment` - Create a new assessment (protected)
- `GET /api/assessment/:id` - Get assessment details (protected)
- `POST /api/submission` - Submit an assessment (protected)
- `GET /api/interview` - Schedule an interview (protected)
- `GET /api/interview/:id` - Get interview details (protected)

# Testing
- Use Jest for unit and integration tests
- Test authentication, assessment creation, submission, and interview scheduling endpoints
- Mock database interactions for isolated testing

