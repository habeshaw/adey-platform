# ADEY — Ethiopian Foreign Exchange Intelligence Platform

Production-grade bilingual (English & Amharic) web application for collecting, archiving, analyzing, and distributing foreign exchange rates from the National Bank of Ethiopia (NBE) and all Ethiopian commercial banks.

## Key Features & Architecture
- **Frontend**: Responsive vanilla JavaScript SPA with Tailwind CSS, bilingual UI switching (English/Amharic), live bank comparison matrix, importer/exporter calculators, and report ordering workflows.
- **Backend & Database**: Supabase PostgreSQL with rigorous Row Level Security (RLS) policies, audit logging, and automated triggers.
- **Automated Collection Engine**: Comprehensive scraper runner supporting NBE and 10+ Ethiopian commercial banks (CBE, Dashen Bank, Bank of Abyssinia, Awash Bank, Cooperative Bank of Oromia, Hibret Bank, Wegagen Bank, Nib International Bank, Zemen Bank, Lion International Bank).
- **Manual Payment Verification & Entitlements**: Telebirr & bank transfer instruction modules, secure receipt submission into private Supabase buckets, and admin review workflows.
- **Paid Document Generation**: Serverless endpoints generating professional Excel (`.xlsx`), PDF (`.pdf`), and Word (`.docx`) reports with secure signed URL access controls.

## Deployment & Configuration Instructions
1. Push all code to your GitHub repository (`adey-platform`).
2. Import the repository into Vercel and verify the **Output Directory** is set to `.` (root).
3. Configure your Supabase environment variables in Vercel (`SUPABASE_URL`, `SUPABASE_SERVICE_ROLE_KEY`).
4. Execute `database/schema.sql` and `database/rls_policies.sql` in your Supabase SQL Editor.
