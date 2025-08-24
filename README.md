# E-Professionals.lk — Full Prototype

Next.js 14 + Tailwind + NextAuth + Prisma (SQLite demo).

## Local setup
```bash
npm i
cp .env.example .env
npm run db:push
npm run db:seed
npm run dev
```
- Admin (seeded): admin@e-professionals.lk / Admin@123

## Deploy (Vercel)
1. Push to GitHub.
2. In Vercel, add env vars:
   - `DATABASE_URL` (use `file:./dev.db` for demo or Postgres URL in production)
   - `NEXTAUTH_SECRET`
   - `NEXTAUTH_URL` (your domain)
3. Run `npm run db:push` and `npm run db:seed` via Vercel CLI or one-off run.
4. Point `www.e-professionals.lk` to Vercel.
