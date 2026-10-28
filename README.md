# Satu Visual Indonesia — Website (testing build)

Single-file website: `index.html` (HTML + Tailwind CSS via CDN + Lucide icons).
No build step needed.

## Publish for testing with GitHub Pages

1. Create a new repository on GitHub, e.g. `satuvisual-website` (Public).
2. Click **Add file → Upload files**, drag in `index.html`, `README.md` and `.nojekyll`, then **Commit changes**.
3. Open **Settings → Pages**.
   - Source: **Deploy from a branch**
   - Branch: **main** / folder **/(root)** → **Save**
4. Wait 1–2 minutes. Your test link will be:
   `https://<your-github-username>.github.io/satuvisual-website/`

## Pages (hash links)

| Page | Link |
|---|---|
| Home | `/#home` |
| NDI Solutions | `/#ndi` |
| About | `/#about` |
| Projects | `/#projects` |
| News & Events | `/#news` |
| Contact | `/#contact` |
| Privacy Policy | `/#privacy` |

## What to test

- Floating WhatsApp button → form → opens WhatsApp to +62 811 804 7717 with the message filled in.
- YouTube thumbnails and inline playback (these work on GitHub Pages; they are blocked in the Claude preview).
- Dark / light toggle, mobile menu, NDI before/after diagram, Telycam tabs, project and news filters.

## Where to edit content (inside `index.html`, in the `<script>` near the bottom)

- `VIDEOS` — YouTube IDs, titles, start time
- `PROJECTS` — project references
- `NEWS` — articles and events
- `PRODUCTS` — product specs shown in the hero and spec panel
- `WA_NUMBER` — WhatsApp number

## Before going live

- Replace placeholders marked `[ ... ]` (project names, photos, talk list, TikTok handle, video titles).
- Swap the temporary wordmark for the official logo file.
- For production, replace the Tailwind CDN script with a compiled Tailwind build (the CDN is meant for prototyping).
- Have the Privacy Policy reviewed by your legal advisor.
