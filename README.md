# Green Klub Monorepo

## Structure

- `apps/api` – Express + Prisma backend
- `apps/web` – React + Vite frontend

## Local Development

1. **Install dependencies:**  
   Run `npm install` from the root.

2. **Backend:**  
   - Add your `.env` file in `apps/api` (see sample).
   - Run migrations (if using Prisma):  
     `cd apps/api && npm run prisma:migrate`
   - Start backend:  
     `npm run dev --workspace=api`  
     (Runs on `localhost:5000`)

3. **Frontend:**  
   - Start frontend:  
     `npm run dev --workspace=web`  
     (Runs on `localhost:5173`)

## Deployment

- Recommended: [Vercel](https://vercel.com/) (both frontend & backend)
- Alternative: Netlify (frontend) + Railway/Fly.io (backend)

## Environment Variables

- `.env` in `apps/api` for backend settings

## Database

- Use PostgreSQL; set your connection string in `.env`
- Run migrations with `npm run prisma:migrate` in `apps/api`

## CI/CD

- See `.github/workflows/deploy.yml` to README.md.