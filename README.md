# SpectrAI 2026 — static event-page prototype

This repository contains a single standalone HTML page (`main.html`) for a proposed SIG RealitySpectra event landing page. It is a **visual/frontend prototype**, not an operational event-registration service.

## Run locally

Open `main.html` in a modern browser. An internet connection is needed to load the externally hosted fonts, icons, and QR-code library. No build system, server, database, or email service is configured.

## Important limitations

- The event date shown in the page is **15 October 2026**, now in the past. The page must not be advertised as accepting current registrations.
- The form only validates browser inputs. Its submit handler prevents the browser submission, displays a success message, and decrements an in-memory counter. **No registration is transmitted, stored, or emailed.**
- The 100-seat display is a hard-coded demonstration counter, **not live inventory**.
- The QR code points to an example destination that has not been independently validated here.
- As of 22 October 2026, the countdown script can throw a `ReferenceError` for an already-passed event date: `updateCountdown()` references `countdownInterval` before its `const` initialization. This prevents subsequent script initialization.
- No CI, automated tests, accessibility audit, or hosted end-to-end registration verification has been established.

**Do not collect real attendee details using this page as-is.** Before publishing a functional registration experience, connect an authorized backend and email workflow, verify the registration URL, use real seat counts, and add a tested closed-registration state. Preserve the existing design and any legitimate contributor/tool attribution when implementing changes.
