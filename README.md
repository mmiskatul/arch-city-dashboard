# Admin Dashboard (Standalone)

Standalone Next.js Admin Dashboard app.

## Local Run

1. Install dependencies:
   - `npm ci`
2. Start dev server:
   - `npm run dev`
3. Open:
   - `http://localhost:3000/admin-dashboard`

## Deploy To Vercel

1. Push this repo to GitHub/GitLab/Bitbucket.
2. In Vercel, click **New Project** and import the repo.
3. Use these settings (already compatible with this repo):
   - Framework: `Next.js`
   - Install Command: `npm ci`
   - Build Command: `npm run build`
4. Add environment variables in Vercel Project Settings if needed.
5. Deploy.

This repo includes `vercel.json` with explicit install/build commands.

## Docker (Optional)

Build image:

```bash
docker build -t admin-dashboard .
```

Run container:

```bash
docker run --rm -p 3000:3000 admin-dashboard
```

Open: `http://localhost:3000/admin-dashboard`

## Included

- Admin routes and pages from `app/admin-dashboard`
- Admin components from `components/admin`
- Admin data modules from `lib/admin`
- Shared route constants in `lib/routes.ts`
- Required Next.js/Tailwind/TypeScript config files
