# Contacts API

A REST API for managing personal contacts, built with Express and PostgreSQL. It provides account registration, JWT-based authentication, email verification, avatar uploads, and protected contact management endpoints.

## Features

- User registration and sign-in
- Email verification and verification email resend
- JWT authentication middleware
- Contact creation, retrieval, update, and deletion
- Joi request validation
- Avatar upload support
- Gravatar-based default avatars
- PostgreSQL persistence through Sequelize
- Centralized HTTP error handling

## Tech stack

- Node.js
- Express
- PostgreSQL
- Sequelize
- JSON Web Tokens
- Joi
- Multer
- Nodemailer

## Getting started

### Prerequisites

- Node.js 18 or later
- PostgreSQL

### Installation

```bash
npm install
cp .env.example .env
```

Configure the environment variables in `.env`, then start the API:

```bash
npm run dev
```

For a production-style start:

```bash
npm start
```

## Project structure

```text
controllers/  Request handlers
db/           Database configuration
decorators/   Reusable controller and validation wrappers
helpers/      Authentication, email, and error utilities
middleware/   Authentication and file-upload middleware
routes/       Express route definitions
schemas/      Joi validation schemas
services/     Business and persistence logic
```

## API areas

- `/api/auth` — registration, login, verification, and account operations
- `/api/contacts` — authenticated contact management

See the route modules for the exact endpoints and request schemas.

