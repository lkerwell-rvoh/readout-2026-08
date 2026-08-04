# Protected documents

Two encrypted static pages:

- `/`      — full research readout
- `/deck/` — discussion deck

Each is AES-256-CBC encrypted with a key derived via PBKDF2-HMAC-SHA256
(6,000,000 iterations) and authenticated with HMAC-SHA256. Decryption happens
client-side in the browser via WebCrypto; the passphrase is never transmitted.

The plaintext is not present in this repository in any form.

Passphrase is distributed separately. Internal use only.
