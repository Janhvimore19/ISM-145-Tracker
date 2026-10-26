# ISM 145 Supabase Cloud Tracker

## What this version removes
- No Python
- No CMD window
- No host laptop
- No office IP
- No SQLite file transfer
- Works from any network through one GitHub Pages link

## One-time setup
1. Create a free Supabase project.
2. Open SQL Editor, paste all of `setup.sql`, and click Run.
3. In Supabase Authentication settings, disable email confirmation for the easiest pilot, or leave it enabled if users can receive confirmation emails.
4. Copy Project URL and Publishable key from Project Settings > API.
5. Paste values into `supabase-config.js`. Never use a secret/service-role key.
6. Upload `index.html`, `app.js`, `supabase-config.js`, and optionally this README to the GitHub Pages repository.
7. Open the GitHub Pages link and create the first accounts.
8. After both TLs create accounts, run the two final UPDATE lines from `setup.sql` with the real TL emails.
9. Refresh and sign in again. TL Approvals appears for TL accounts.

## Password reset
The Forgot Password button sends a Supabase reset email. Add the GitHub Pages URL under Authentication > URL Configuration > Redirect URLs.

## Notes
- New employee accounts begin with Casual Leave 14, Earned Leave 0, Maternity Leave 182. A TL balance-management module can be added next.
- This package does not migrate the old SQLite data automatically.
- Use the publishable key in the browser. Never upload the secret/service-role key.
