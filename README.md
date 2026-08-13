# Protected documents

Ten encrypted static pages, in two groups.

**2027 strategy**

- `/` — full research readout
- `/deck/` — discussion deck
- `/strategy/` — PM strategy

**Maintenance phase**

- `/maintenance/dashboard/` — index of everything below, start here
- `/maintenance/kickoff/` — kickoff deck, 18 slides
- `/maintenance/` — clickable prototype, 23 annotated screens
- `/maintenance/prd/` — creative brief and PRD (draft)
- `/maintenance/synthesis/` — the synthesis
- `/maintenance/language/` — member-facing copy and house style
- `/maintenance/canvas/` — value proposition canvas

Each page is AES-256-CBC encrypted with a key derived via PBKDF2-HMAC-SHA256
(6,000,000 iterations) and authenticated with HMAC-SHA256. Decryption happens
client-side in the browser via WebCrypto; the passphrase is never transmitted.

The plaintext is not present in this repository in any form.

Passphrase is distributed separately. Internal use only.
