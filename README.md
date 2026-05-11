# Best Polity LLC — Client Proposal Portal

Secure, password-gated document delivery and e-signature portal for Best Polity LLC managed services clients.

## Features

- **Password-protected document portal** — single-use access code per client
- **Live proposal delivery** — branded with Best Polity identity
- **Statement of Work (PDF)** — downloadable, CPA-ready with tax code citations
- **Executive IT Dashboard preview** — asset inventory, network topology, subscription tracking
- **E-signature acceptance** — freehand signature pad with CAPTCHA verification
- **Timestamped acceptance record** — stored locally, verifiable by both parties
- **Tax treatment references** — IRC §162, NY Tax Law §208/§612 linked

## Tech Stack

- Pure HTML/CSS/JS (zero dependencies)
- Canvas-based signature pad (mouse + touch + stylus compatible)
- GitHub Pages hosting
- No backend, no database, no API keys
- All state in localStorage

## Usage

1. Deploy to GitHub Pages
2. Set `CORRECT_PASSWORD` in the HTML
3. Update proposal content for each client
4. Send client the URL and access code

## Structure

```
/
├── index.html                     # Client portal (lock screen + proposal + e-sign)
├── dashboard-preview.html         # Executive IT Dashboard preview
└── Statement-of-Work-Best-Polity-LLC.pdf  # SOW deliverable
```

## Security

- Passwords set per-client, changeable between engagements
- No data transmitted to external servers
- Acceptance records stored client-side only
- CAPTCHA prevents automated acceptance
- Touch-safe with `touch-action: none` and `user-select: none`

## SOP Reference

See Best Polity LLC internal SOP-013: Managed Services Delivery Protocol for full engagement lifecycle.

---

**Best Polity LLC** · william@bestpolity.com
