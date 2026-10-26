# ISM 145 Exact-Design Supabase Cloud Tracker

This package preserves the supplied final dashboard design and replaces only the Python/SQLite backend with Supabase.

## Files to upload to GitHub Pages
- `index.html`
- `supabase-config.js`

## One-time Supabase update
1. Open Supabase SQL Editor.
2. Paste all of `setup_exact_dashboard.sql`.
3. Click Run. Expected result: Success, no rows returned.
4. In Authentication settings, disable Confirm email for the easiest pilot, or let users confirm their email before first sign-in.

## Configure
Copy your already edited Supabase values into this package's `supabase-config.js`.
Use only the browser-safe Publishable key, never the secret/service-role key.

## GitHub
Replace the repository's existing `index.html` and `supabase-config.js` with these files.
Delete the simplified pilot `app.js`, because the exact dashboard JavaScript is embedded inside this `index.html`.
Keep `README.md` optional.

## Login
Each registered email selects its email and enters a separate tracker password.
The first attempt creates the Supabase Auth account if it does not already exist.
Both registered TL emails automatically open the TL dashboard in the interface.

## Included exact-design modules
- Employee dashboard
- Shared TL dashboard
- Monthly Team Planner
- Annual calendar
- Requests and Outlook drafts
- Leave balance management
- Past leave entry and CSV import
- Reply reminders
- Utilization chart
- Account/password change
