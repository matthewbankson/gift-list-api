# Gift List API

A RESTful API for tracking gift lists, built with Fastify, TypeScript, and PostgreSQL.

## Tech Stack

- **Runtime**: Node.js with TypeScript
- **Framework**: [Fastify](https://www.fastify.io/) - Fast and low overhead web framework
- **Database**: PostgreSQL 17
- **ORM**: [Drizzle ORM](https://orm.drizzle.team/) - TypeScript ORM
- **Linting/Formatting**: [Biome](https://biomejs.dev/) - Fast formatter and linter
- **Containerization**: Docker & Docker Compose

## Prerequisites

- Node.js (v14.21.3 or higher)
- npm or yarn
- Docker and Docker Compose

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/matthewbankson/gift-list-api.git
cd gift-list-api
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Create a `.env` file in the root directory:

### 4. Start the database

```bash
docker-compose up -d
```

This will start a PostgreSQL 17 container with:
- Database: `gift_list`
- User: `postgres`
- Password: `postgres`
- Port: `5432` (or as configured in docker-compose.yaml)

### 5. Run database migrations

```bash
npx drizzle-kit push
```

### 6. Build the project

```bash
npm run build
```

### 7. Start the server

```bash
npm start
```

The API will be available at `http://localhost:8080`

## Author

matthewbankson
