# Quick Setup Guide

## Environment Variables Setup

1. Create a `.env.local` file in the root directory
2. Add your Supabase credentials:

```bash
NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
```

## Quick Test

Visit `/quick-test` to check if your environment variables are set correctly.

## Database Setup

Run the SQL scripts in the `scripts/` folder in order:
1. `01-create-tables.sql`
2. `02-create-policies.sql`
3. `05-create-faculty-gallery-tables.sql`
4. `07-create-enquiries-table.sql`
5. `04-seed-data.sql`
6. `06-seed-faculty-gallery-data.sql`

## Common Issues

- **Empty error object {}**: Usually means missing environment variables
- **Institute not found**: Check if institutes exist and are active
- **RLS policy errors**: Make sure policies are created correctly

