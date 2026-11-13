# ADEY — Ethiopian Foreign Exchange Intelligence Platform

Production-grade bilingual (English & Amharic) web application for collecting, archiving, analyzing, and distributing foreign exchange rates from the National Bank of Ethiopia (NBE) and all Ethiopian commercial banks, with automated daily Vercel Cron data collection.

## Quick Setup Instructions
1. **Supabase Database**: Run `database/schema.sql` and `database/rls_policies.sql` in your Supabase SQL Editor.
2. **Frontend Configuration**: Open `index.html` and update `SUPABASE_URL` and `SUPABASE_ANON_KEY` with your actual project credentials.
3. **Environment Variables on Vercel**: Set `SUPABASE_URL` and `SUPABASE_SERVICE_ROLE_KEY`.
4. **Deploy**: Push to GitHub and import into Vercel (Root Output Directory: `.`).
