# Hyatt AI Tool Governance — Concept Sites

Static concept mock-ups for the AI Tool Governance hub on Hyatt Connect.
No build step, no dependencies — every page is a self-contained HTML file.

## Pages
- `index.html` — landing page linking to all three options
- `option-a/` — **Adoption Gallery** (community-led; includes a working in-session story submission flow)
- `option-b/` — **Governance Registry** (system-of-record-led)
- `option-c/` — **CoE Command Center** (operating-model-led)

## Deploy (Vercel)
1. Push this folder's **contents** to a new GitHub repo (so `index.html` is at the repo root).
2. In Vercel: **Add New → Project → Import** the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Deploy.

Live URLs:
- Hub: `https://<your-project>.vercel.app/`
- `…/option-a/`, `…/option-b/`, `…/option-c/`

## Notes
- Fonts render as **Segoe UI** on Windows/SharePoint (Arial fallback elsewhere).
- Hero/logo imagery are placeholders pending official Hyatt assets.
- Interactivity (navigation, filters, the Option A submission flow) runs fully client-side.
  Data is **not** persisted across visitors — the production target is SharePoint lists + Power Automate.
