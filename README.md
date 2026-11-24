# OpsGrid

OpsGrid is an IT operations console for monitoring and managing alerts,
incidents, activity, analytics, automation, workspaces, and connected computers.

## Required backend

This app requires the main [Base44 Supabase Setup](https://github.com/zzz-creator/base44-supabase-setup)
repository to run its self-hosted Supabase backend. Do not clone this app alone
when setting up a new environment; clone the main repository with its
submodules:

```sh
git clone --recurse-submodules https://github.com/zzz-creator/base44-supabase-setup.git
```

Follow the main repository's [fresh setup instructions](https://github.com/zzz-creator/base44-supabase-setup#fresh-setup)
to configure and start Supabase. Create this app's `.env.local` with
`VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY` from that backend. For a
local stack, the URL is typically `http://localhost:8000`. Use only the public
anon key in the frontend, never the service-role key.

## Run locally

From the `OpsGrid` directory:

```sh
npm install
npm run dev
```

Available checks: `npm run lint`, `npm run typecheck`, and `npm run build`.
