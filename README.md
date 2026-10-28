# UIC Org Events

Public student organization calendar: https://shazaibdawood.github.io/uic-org-events/

This repository contains the public frontend only. The calendar, events, connections, Google authorization, and scheduled synchronization remain in the existing Google Calendar / Apps Script backend. No Google OAuth credentials are stored in this repository.

Visitors can subscribe to the shared Google Calendar, add or edit site-created events, and connect an accessible organization calendar. Imported events are updated at their source and sync about every 15 minutes. Times use America/Chicago.

## Hosting

GitHub Pages publishes the root of `main`. `.nojekyll` disables Jekyll processing. No paid domain, server, build service, or API key is required for this frontend. Keep this repository public and Pages enabled. GitHub's hosting terms and limits apply; this is not a contractual uptime guarantee.

The canonical local project builds this `index.html` with `node build.mjs` and verifies backend behavior with `node verify.mjs`. After updating the frontend, commit and push the generated file to `main`.

The existing Sites URL remains supported by the Google backend during migration. Google data is independent of both frontend hosts.
