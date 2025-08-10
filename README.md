# Green Klub

Premium Cannabis Microbusiness Website  
Full-stack, mobile-first site for education, cultivation, and product sales.

## Structure

- **Frontend:** Next.js + Tailwind CSS (`apps/web`)
- **Backend:** Node.js + Express (`apps/api`)
- **Database:** PostgreSQL (Prisma ORM, `prisma`)
- **CMS:** Sanity/Strapi (to be added)
- **Hosting:** Vercel (frontend), Render/Supabase (backend)

## Getting Started

### Frontend

```sh
cd apps/web
npm install
npm run dev
```

### Backend

```sh
cd apps/api
npm install
npm run dev
```

### Database

Configure PostgreSQL connection in `.env` and run:
```sh
npx prisma migrate dev
```