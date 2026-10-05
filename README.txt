KNIGHT FRANK – TOPIC OF THE DAY
LIVE MVP

What this version does:
- Loads today's active question from Supabase.
- Lets colleagues click A or B.
- Saves the anonymous vote to Supabase.
- Shows live totals and percentages.
- Shows the Fun Fact.
- Returns to the question after 8 seconds.
- Checks once per minute for a new day's question.
- Uses the supplied Knight Frank logo.

IMPORTANT:
1. Open index.html in a text editor.
2. Find:
   const SUPABASE_URL = "PASTE_YOUR_PROJECT_URL_HERE";
   const SUPABASE_PUBLISHABLE_KEY = "PASTE_YOUR_PUBLISHABLE_KEY_HERE";
3. Paste your Supabase Project URL and Publishable key there.
4. Never paste a Supabase Secret key / service_role key.
5. Save index.html.
6. Open it in Chrome to test.

For the first live test before 24 Aug:
The app uses the real current date. If you want to test the 24 Aug question before launch,
temporarily replace:
   const today = localDateISO();
with:
   const today = "2026-08-24";
Then change it back before launch.

Deployment:
This is a plain static HTML site, so it can be deployed to Vercel, Netlify, GitHub Pages,
or another static host. Vercel is a convenient choice.

Next phase after the TV MVP:
- Admin login
- Admin page for adding/editing questions
- Better anti-repeat voting behavior if desired
- Custom company URL
