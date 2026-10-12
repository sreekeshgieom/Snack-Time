# Snack Time

A cheerful SvelteKit dashboard for tracking chai, coffee, milk, and snacks twice a day. Admins can fill in missed entries, edit past days, and remove duplicates. Built with SvelteKit, Prisma, and MySQL.

## Features
- Morning + evening log with sugar, milk, and snack count choices.
- Backdate entries to cover missed days.
- Monthly summary view with quick stats.
- Admin controls for marking entries on behalf of users.

## Quick start

```bash
npm install
npm run dev
```

## Database setup (MySQL via Docker)

```bash
docker compose up -d
cp .env.example .env
npm run db:push
```

## Prisma schema
See `prisma/schema.prisma` for enums and data model.
