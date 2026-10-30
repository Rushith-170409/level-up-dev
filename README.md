# Level Up — Development v0.3

This is a development build of the Level Up PWA. It is separate from the live GitHub Pages app.

## Included in this build
- Existing habits, measurable goals, focus logging, XP ledger, daily review and JSON backup/restore.
- Habit analytics: completion totals, streak estimates, 28-day heatmap and per-habit rates.
- Weekly report generation, local report archive and browser Print → Save as PDF.
- Sleep/wake planning and a Google Calendar reminder-template handoff. The reminder is not a guaranteed alarm.
- Timestamped daily reflection save and existing activity log.
- Clearly marked setup panels for Google Calendar and Level Up Intelligence.

## Not connected yet (requires secure backend / external setup)
- Google Calendar OAuth and two-way sync. No calendar data is read or written by this build.
- AI personal coach and planning assistant. A server-side AI endpoint and API key management are required; never put an API key in public JavaScript.
- Native/reliable alarms, push notifications and guaranteed background execution. A PWA cannot promise these when closed or suspended.
- Server-side anti-cheat, accounts, cloud sync and immutable audit storage. Browser localStorage can be edited or deleted by the device owner.

## Important testing note
This build uses the development storage key `levelup-pwa-dev-v2`; it does not automatically import or overwrite the production app's local data. Export a backup from the live app before any future migration. Do not replace the production repository with this build until migration and testing are complete.

## Run locally
Serve this folder over localhost (for example with VS Code Live Server) or publish it to a separate GitHub repository with GitHub Pages. Opening `index.html` directly may disable PWA service-worker features.

## Deployment
Upload the contents of this folder (not the enclosing folder) to the root of a separate development repository. Enable GitHub Pages for the main branch/root. Test install, offline reload, backup/restore and all controls on both desktop and Android before considering production.
