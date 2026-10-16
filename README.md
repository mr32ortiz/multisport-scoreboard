# MLB-style Multi-Sport Overlay

- `index.html`: compact, transparent, top-left overlay in navy, white, and subtle gold.
- `control.html`: remote controller with editable full team names, softball scores/inning/count/outs/base runners, and pickleball scores/serving team/server number/game number.

## Update GitHub Pages
Upload `index.html`, `control.html`, and `README.md` directly to the **root** of your existing GitHub repository, replacing the existing files, then commit changes. Keep your current repository and Pages settings.

## Connect live scores with Supabase
1. Create a Supabase project.
2. Copy the Project URL and public publishable/anon key from the project API settings.
3. Open the controller, enter URL/key and a room code (default `matchday`), then press Connect.
4. Open the overlay URL with matching query parameters: `https://YOUR-USERNAME.github.io/YOUR-REPO/?url=YOUR_SUPABASE_URL&key=YOUR_PUBLIC_KEY&room=matchday`. URL-encode values if needed.

Never use a service-role or secret key in browser pages. This prototype uses realtime broadcast and does not save game history. Keep the controller open during a stream and test both pages before going live. Streamlabs Mobile support for custom browser/URL overlays varies by app/version.
