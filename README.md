# Protected documents

Fifteen encrypted static pages, in two groups.

**2027 strategy**

- `/` — full research readout
- `/deck/` — discussion deck
- `/strategy/` — PM strategy

**Maintenance phase** — start at the dashboard, which links to everything else

- `/maintenance/dashboard/` — index of everything below
- `/maintenance/kickoff/` — kickoff deck, 18 slides
- `/maintenance/` — clickable prototype, 23 annotated screens
- `/maintenance/mvp/` — MVP prototype, 18 screens, scoped for 3/1
- `/maintenance/design-brief/` — product design brief
- `/maintenance/mvp-design-brief/` — MVP product design brief
- `/maintenance/prd-draft/` — north-star PRD draft
- `/maintenance/mvp-prd-draft/` — MVP PRD draft
- `/maintenance/synthesis/` — research synthesis
- `/maintenance/language/` — member-facing copy and house style
- `/maintenance/lifecycle/` — lifecycle and marketing plan
- `/maintenance/canvas/` — value proposition canvas

`/maintenance/prd/` redirects to `/maintenance/design-brief/`. The creative brief and PRD became the
product design brief; the technical PRD is a separate document.

Each page is AES-256-CBC encrypted with a key derived via PBKDF2-HMAC-SHA256
(6,000,000 iterations) and authenticated with HMAC-SHA256. Decryption happens
client-side in the browser via WebCrypto; the passphrase is never transmitted.

The plaintext is not present in this repository in any form.

Passphrase is distributed separately. Internal use only.
