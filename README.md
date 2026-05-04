# Next.js Docker App

This is a Next.js application with Docker setup, connected to PostgreSQL from Neon.tech.

## Getting Started

### Prerequisites

- Docker installed on your machine

### Running the Application

1. Build the Docker image:

   ```bash
   docker build -t nextjs-docker-app .
   ```

2. Run the container:

   ```bash
   docker run -p 3000:3000 nextjs-docker-app
   ```

3. Open [http://localhost:3000](http://localhost:3000) in your browser.

The application will test the database connection and display the current time from PostgreSQL.

## Environment Variables

The database connection is configured via the `DATABASE_URL` environment variable in `.env.local`.

## Development

If you want to run in development mode without Docker:

1. Install dependencies:

   ```bash
   npm install
   ```

2. Run the development server:
   ```bash
   npm run dev
   ```

Make sure to set the `DATABASE_URL` in your environment.
