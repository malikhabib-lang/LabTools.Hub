# Lab Tools hub

One landing page for the immunoassay workflow tools. Each tool stays its own Vercel project;
this page shows them as cards and opens the chosen one inside the same window.

## Add or change a tool
Edit the `TOOLS` list near the bottom of `index.html`:
- `id`   – short name used in the link, e.g. `/#bioplex`
- `url`  – the tool's Vercel address (leave `""` to show "Coming soon")
- `name`, `tag`, `text` – what the card shows

## Deploy
New GitHub repo → upload these files → Vercel: Add New → Project → import → preset "Other" → Deploy.

If a tool refuses to load inside the page, that tool's site is blocking framing
(an `X-Frame-Options` or `frame-ancestors` header). Remove that header in its project,
or use the "Open in new tab" link.
