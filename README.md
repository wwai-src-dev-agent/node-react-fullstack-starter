# Node React Fullstack Starter

This repository contains a basic full‑stack web application template using **Next.js** for the front‑end and **Express** with **Prisma** for the back‑end. The goal of this starter is to provide a clean, modern foundation for building web applications with separate front‑end and back‑end services using TypeScript.

## Structure

* `frontend/` – A [Next.js](https://nextjs.org/) application (TypeScript) for the user interface. It comes with a simple landing page and is preconfigured for Tailwind CSS.
* `backend/` – An [Express](https://expressjs.com/) server that exposes a basic API endpoint. It’s written in TypeScript and uses Prisma for database access.
* `prisma/` – The Prisma schema and configuration. Update the model definitions here and run migrations to evolve your database schema.

## Getting started

1. **Install dependencies**

   From the repository root:

   ```bash
   # install dependencies for all workspaces
   npm install
   ```

2. **Configure the database**

   Set the `DATABASE_URL` environment variable in `backend/.env` for Prisma. For example:

   ```
   DATABASE_URL="postgresql://user:password@localhost:5432/mydb"
   ```

3. **Run Prisma migrations**

   ```bash
   cd backend
   npx prisma migrate dev --name init
   ```

4. **Start the backend**

   ```bash
   cd backend
   npm run dev
   ```

5. **Start the frontend**

   In a separate terminal:

   ```bash
   cd frontend
   npm run dev
   ```

6. **Access the application**

   Visit `http://localhost:3000` in your browser for the front‑end and `http://localhost:3001/api/hello` for the back‑end API.

## Notes

This template is a starting point meant to be customized. You can add additional routes, pages, database models, or third‑party integrations as needed. Happy hacking!
