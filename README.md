# Lead Tracker

Static site, no build step. Everything served lives in `public/`.

## Deploy on Cloudflare
1. Create a new GitHub repo and upload the contents of this folder (README.md, wrangler.jsonc, public/).
2. Cloudflare dashboard -> Workers & Pages -> Create -> import the repo.
   - Build command: leave empty
   - If it asks for a build output directory (Pages): `public`
   - If it deploys as a Worker, `wrangler.jsonc` already points at `public/` - nothing to set.

## Install as a Mac app
Open the deployed URL in Chrome -> menu -> Cast, save and share -> Install page as app.
Then link `leads.xlsx` once (Open my leads Excel file).

Your leads are stored only in the Excel file on your computer, never on Cloudflare.
