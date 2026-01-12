# Bachelor Project - NestJS Backend

**Description**  
This is a bachelor project backend built with NestJS, featuring REST and WebSocket APIs, JWT authentication, a real-time chat, Prisma ORM, Redis caching, and Cloudinary integration.

---

## Features

- NestJS framework
- JWT Authentication (Access & Refresh tokens)
- WebSocket chat support
- Prisma ORM for PostgreSQL
- Redis caching
- Cloudinary integration for media
- CRUD operations for users and notes

---

## Installation

1. **Clone the repository**

```bash
git clone git@github.com:MikroTik2/bachelor.git
cd bachelor
```

2. **Clone the repository**


```bash
npm install
```

3. **Create .env file**

Create a .env file in the root of the project and add the following environment variables:

```bash
# Node environment
NODE_ENV='development'

# HTTP configuration
HTTP_PORT=4000
HTTP_HOST='http://localhost:4000'
HTTP_CORS='http://localhost:3000/,http://localhost:14701/'

# PostgreSQL database
POSTGRES_USER='<YOUR_DB_USER>'
POSTGRES_PASSWORD='<YOUR_DB_PASSWORD>'
POSTGRES_HOST='<YOUR_DB_HOST>'
POSTGRES_PORT=<YOUR_DB_PORT>
POSTGRES_DB='<YOUR_DB_NAME>'
POSTGRES_URI='postgresql://<YOUR_DB_USER>:<YOUR_DB_PASSWORD>@<YOUR_DB_HOST>:<YOUR_DB_PORT>/<YOUR_DB_NAME>?schema=public'

# Redis configuration
REDIS_USER='<YOUR_REDIS_USER>'
REDIS_PASSWORD='<YOUR_REDIS_PASSWORD>'
REDIS_HOST='<YOUR_REDIS_HOST>'
REDIS_PORT=<YOUR_REDIS_PORT>
REDIS_URI='rediss://<YOUR_REDIS_USER>:<YOUR_REDIS_PASSWORD>@<YOUR_REDIS_HOST>:<YOUR_REDIS_PORT>'

# Cookie configuration
COOKIE_SECRET='<YOUR_COOKIE_SECRET>'
COOKIE_DOMAIN='localhost'

# JWT configuration
JWT_SECRET='<YOUR_JWT_SECRET>'
JWT_ACCESS_TOKEN_TTL='2h'
JWT_REFRESH_TOKEN_TTL='7d'

# Cloudinary
CLOUDINARY_API_KEY='<YOUR_CLOUDINARY_API_KEY>'
CLOUDINARY_API_SECRET='<YOUR_CLOUDINARY_API_SECRET>'
CLOUDINARY_API_NAME='<YOUR_CLOUDINARY_NAME>'
```

5. **Seed the database (optional)**

```bash
npm run db:seed
```

## Running the project

Development mode (watch mode):

```bash
npm run start:dev
```

Production mode

```bash
npm run build
npm run start:prod
```

Debug mode:

```bash
npm run start:debug
```