# ADEY Financial Intelligence Platform — Deployment Guide

ADEY is a secure, data-driven financial intelligence platform for the Ethiopian foreign-exchange (FX) market. It features automated rate collection, role-based access control, manual payment verification (Telebirr & Bank Transfer), and secure entitlement management.

---

## Step-by-Step Deployment Instructions

### Step 1: Set Up Supabase Project
1. Log in to your [Supabase Dashboard](https://supabase.com) and create a new project.
2. Go to the **SQL Editor** on the left sidebar.
3. Run the complete SQL migration script located in `database/schema.sql`.
4. Run the Row Level Security (RLS) policies script located in `database/rls_policies.sql`.
5. Create two **Private** storage buckets in Supabase Storage:
   - `payment-receipts`
   - `premium-reports`
6. Copy your Supabase Project URL (`SUPABASE_URL`) and Service Role / Anon Keys from **Project Settings > API**.

### Step 2: Push to GitHub
1. Initialize a Git repository in this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial ADEY platform deployment commit"
   ```
2. Create a new repository on GitHub and push your code:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/adey-platform.git
   git branch -M main
   git push -u origin main
   ```

### Step 3: Deploy to Vercel
1. Log in to [Vercel](https://vercel.com) and click **Add New > Project**.
2. Import your GitHub repository (`adey-platform`).
3. Configure **Environment Variables** in Vercel before deploying:
   - `SUPABASE_URL`: Your Supabase project URL
   - `SUPABASE_SERVICE_ROLE_KEY`: Your Supabase service role secret key
4. Click **Deploy**. Vercel will automatically build and publish your serverless API routes and static frontend.
