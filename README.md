# ADEY Financial Intelligence Platform — Deployment Guide

ADEY is a secure, data-driven financial intelligence platform for the Ethiopian foreign-exchange (FX) market.

## Features Included
- Fully functional frontend Single Page Application (SPA) with user registration, login, customer dashboard, and admin management console.
- Supabase Authentication & Row Level Security (RLS).
- Live Ethiopian FX rates preview and administrative data management.

## Deployment Instructions (Vercel & GitHub)
1. Push all files in this repository to your GitHub repository (`adey-platform`).
2. Import the repository into Vercel.
3. In Vercel Project Settings -> Build and Deployment, ensure **Output Directory** is set to override as `.` (root).
4. Configure environment variables in Vercel if needed (`SUPABASE_URL`, `SUPABASE_SERVICE_ROLE_KEY`).
5. Deploy!
