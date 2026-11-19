FATIMA AZAHARIOU PORTFOLIO

FILES
- index.html: portfolio website
- config.js: Supabase browser configuration (fill in after setup)
- supabase-setup.sql: database table and security policies

PUBLISHING WITH GITHUB PAGES
1. Create a public GitHub repository named fatima-portfolio.
2. Upload index.html, config.js, and this README at the repository root.
3. In repository Settings > Pages, deploy from branch main, folder /(root).

ENABLE REAL RECOMMENDATIONS (ONE-TIME SETUP)
1. Create a project at https://supabase.com/ and open its SQL Editor.
2. Paste the contents of supabase-setup.sql and run it.
3. In Project Settings > API (or Connect), copy the Project URL and anon/public key.
4. Open config.js and replace YOUR_SUPABASE_PROJECT_URL and YOUR_SUPABASE_ANON_KEY.
5. Upload the updated config.js to GitHub. Never put a service_role or secret key in this website.
6. Test a recommendation submission. It should be saved with status=pending.
7. To approve: Supabase Dashboard > Table Editor > recommendations; change status to approved.
   Approved recommendations then appear on the website. Rejected/pending ones stay private.

IMPORTANT
- The database policies allow public inserts only as pending and public reads only when approved.
- Keep the Supabase service_role key private.
- For stronger spam protection before sharing widely, add CAPTCHA / rate limiting (e.g. Cloudflare Turnstile plus a server-side verification function).
- Replace YOUR_EMAIL@example.com in index.html with your real professional email address.
- Review all claims, links, dates, and metrics before publishing.
