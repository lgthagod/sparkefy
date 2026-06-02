# Sparkefy Support Site

This is the official short support page for the Sparkefy iOS app (Car Detailing • Boat Cleaning • Lawn Care marketplace).

**Primary short URL (GitHub Pages):**  
https://lgthagod.github.io/sparkefy

**Alternative short URL (recommended for branding):**  
https://sparkefy-support.vercel.app  (or your chosen slug)

## Why this exists
App Store Connect **requires** a public Support URL (and usually a Privacy URL) that:
- Is live and reachable over HTTPS
- Contains real contact information (email or form) so users can reach you about the app
- Is **not** just an FAQ with no contact method

See: App Store Connect Help > App Information.

This page satisfies the requirement with:
- Prominent `mailto:sparkefysupport@gmail.com`
- Short, accurate answers to the most common in-app questions
- A compact privacy/terms summary (so the same URL or `#privacy` anchor can be used for the Privacy URL field)

## How to deploy / get your short URL (pick one)

### Option A — GitHub Pages (already published via this repo)
1. The files in this folder are pushed to the `sparkefy` repo.
2. Go to https://github.com/lgthagod/sparkefy → **Settings → Pages**
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: `main` / `(root)`
4. Save. The site will be live at `https://lgthagod.github.io/sparkefy` within ~30-60 seconds.
5. Paste that exact URL into App Store Connect → your app → App Information → **Support URL** (and optionally Privacy URL).

### Option B — Vercel (often gives the nicest short branded slug)
1. Go to https://vercel.com
2. "Add New Project" → "Import Git Repository" (point at the `sparkefy` repo) **or** simply drag the entire `Sparkefy-Support` folder onto the Vercel dashboard (no Git required).
3. Vercel will give you a URL like `https://sparkefy-support.vercel.app` (or `sparkefy-xxx.vercel.app`).
4. You can rename the project in Vercel settings for a clean slug.
5. Use the Vercel URL as your Support URL (many people prefer the `.vercel.app` look for apps).

### Option C — Netlify / other one-click
- Drag the folder onto https://app.netlify.com/drop
- Or use Tiiny Host, Surge, etc.
- Any of them will give you a working public URL in seconds.

## Updating the URL later
1. Edit the constant in the iOS app:
   `V3Sparkefy/Services/Config.swift` → `supportURL`
2. (If you want the footer on the site to match) edit `index.html` footer.
3. Re-deploy the site (GitHub/Vercel/etc.).
4. Update the two places in App Store Connect (Support URL + Privacy URL). No new binary needed.

## In-app usage
The Profile tab now has a "Support & Legal" section that opens this page directly (uses the value from `Config.supportURL`).

## Contact email used on the site
`sparkefysupport@gmail.com` (matches the demo user pattern `*@sparkefy.app` used throughout the app).

## Notes for App Store submission
- This page is intentionally minimal and mobile-friendly.
- It contains a real email + contact instructions + short legal summary.
- Reviewers will open the Support URL from the App Store listing after purchase.
- You can improve the page (add a real form, more copy, your logo PNG, etc.) at any time without affecting the binary.

Good luck with the submission! 🚀

— Built as part of Sparkefy App Store readiness work.