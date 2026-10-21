# SpectrAI 2026 — static event-page prototype

This repository contains a single static HTML page (`main.html`) for a SIG RealitySpectra event concept. It is a frontend demonstration, **not an operational registration or ticketing service**.

## Implemented

- Responsive page layout, countdown, form-field validation, and local visual feedback.
- A browser-only seat-count display and a QR-code library loaded from a public CDN.

## Not implemented or verified

- **No registration backend or database.** Form submissions are not sent to an API or saved as registrations.
- **No email delivery.** The current success toast says to check email, but no confirmation email is sent.
- **No authoritative seat inventory.** The seat count changes only in the browser and must not be treated as an available-capacity guarantee.
- No automated CI/build or end-to-end validation is configured in this repository.
- Event date, venue, availability, and registration-opening claims in the static page have not been independently verified.

**Do not distribute this page as a live registration link.** Before accepting actual participants, connect a consent-aware registration backend, implement delivery/error handling and privacy notices, make seat inventory authoritative, and replace the current success messaging. Keep applicant contact details out of the public repository.

## Local preview

Open `main.html` in a browser. Internet access is needed for the linked external fonts, icons, and QR-code library. No package installation is required.

## Attribution

Third-party fonts, Font Awesome icons, and the QRCode.js CDN library are used as external dependencies; retain their respective notices and licenses. Do not represent those third-party components as original work.
