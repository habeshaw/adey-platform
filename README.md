# ADEY Financial Intelligence Platform — Deployment Guide

ADEY is a secure, data-driven financial intelligence platform for the Ethiopian foreign-exchange (FX) market.

## Deployment Instructions
1. Push this folder to your GitHub repository (`adey-platform`).
2. Import the repository into Vercel.
3. In Vercel Project Settings -> Build and Deployment, ensure **Output Directory** is set to override as `.` (root).
4. Configure environment variables in Vercel:
   - `SUPABASE_URL`
   - `SUPABASE_SERVICE_ROLE_KEY`
5. Deploy!
