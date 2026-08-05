# AVITAN — Privacy Policy

*Last updated: 2026-08-05*

## In one sentence

AVITAN is a **local-first** companion: almost everything you tell it stays
on your phone, in a private on-device database. It does not require an
account, does not sell data, and never shows ads.

## 1. What AVITAN collects

| Data | What it is | Where it lives |
|---|---|---|
| Your chat text | The messages you type in the Chat tab | On-device database only |
| Extracted tracking data | Money, attendance, schedule, goals, sleep, screen-time logs that you confirm | On-device database only |
| Health readings (optional) | Blood sugar, blood pressure, heart rate, weight, steps — logged by you in chat or synced read-only from Google Health Connect | On-device database only |
| Your notes (optional) | Notes you write or save from chat ("remember that…") | On-device database only |
| Notification summaries (optional) | Titles and bodies of app notifications, with names and phone numbers **redacted on-device** before storage | On-device database only |
| Screen-time stats (optional) | Which apps you use and for how long | On-device database only |
| Anonymous usage analytics (optional) | Event counts only (e.g. "app opened", "money entry confirmed") — **never** message content or names | On-device, then sent as day-old digests to our AI proxy only if you opt in |

## 1a. Health Connect sync (optional)

- With your explicit consent, AVITAN can **read** blood sugar, blood
  pressure, heart rate, weight and steps from Google Health Connect (the
  data apps and wearables on your phone collect).
- This is **read-only**: AVITAN never writes, edits or deletes data in
  Health Connect.
- Synced readings are stored **only in the on-device database** — they are
  never uploaded, sold or shared with anyone.
- You control this at any time: a **Disconnect** button inside the app, or
  the Health Connect app's own permission screen, where you can also
  revoke each data type individually.
- The optional "hourly background sync" reads new readings in the
  background only if you enable it and grant it in the Health Connect app.

## 1b. Health alerts (optional, on-device)

- When you enable **Health alerts**, AVITAN checks every new reading
  against fixed thresholds — blood sugar below 70 mg/dL, above 250 mg/dL,
  or blood pressure at 180/120 or higher.
- Alerts are computed **entirely on your device**: a full-screen alarm for
  low blood sugar, a sound notification for the other two. No AI is
  involved and no data leaves the device to decide an alert.
- The alerts toggle is in the Health tab → Readings, and you can turn it
  off at any time.

## 2. Where your data lives

- **All core data is stored in a private SQLite database on your device.**
  Nothing is uploaded to any cloud by default.
- Android may back your app data up to your Google account (Auto Backup)
  when your phone is idle; restoring to a new phone brings your data back.
- You can also export a backup file yourself from Settings → Backup & restore.

## 3. Cloud AI calls

When you use AI chat (via the optional subscription), only the following
leaves your device:

1. Your current message.
2. A short summary of context relevant to answering it (recent activities,
   schedule, profile, financial/attendance summaries, and — only for
   explicit "do you remember…" questions — a limited set of matching past
   records from your own device).

Your raw chat history is never uploaded. AI requests go through our proxy,
which does not store message content and which you must access with a paid
subscription license.

## 4. Third parties

| Service | Purpose | Data shared |
|---|---|---|
| Google Play | Subscription billing (₹299/month, optional) | Purchase tokens (Google only, never us) |
| AVITAN AI proxy (our own server) | Routing AI requests for subscribers | Your message + context summary; no message storage |
| DeepSeek (our AI provider) | Generating AI replies | Your message + context summary (via our proxy) |
| Sentry (optional) | Crash reporting — only if the developer enables it in the build | Anonymous device/stack-trace data, no personal data |
| Google Play Games/services (Android OS) | Standard OS services | Per Android OS policy |

## 5. Retention

- On-device data is kept until you delete it (per-entry or the in-app
  "wipe all data" button) or delete the app.
- Analytics digests on our proxy are retained for 30 days and contain no
  personal data.
- No account, email, or phone number is ever collected or stored by us.

## 6. Your controls

- **Wipe all data**: Settings → wipe button (instant, irreversible).
- **Backup / restore**: Settings → Backup & restore (manual export/import).
- **Disable capture**: turn off notification insights, screen-time, money or
  attendance tracking at any time in Settings.
- **Health Connect**: connect/disconnect in the Health tab; each data type
  can be revoked individually in the Health Connect app.
- **Decline analytics**: keep "Anonymous usage analytics" off (it is off by
  default).
- **Delete the app** removes all on-device data.

## 7. Children's privacy

AVITAN is designed for users 13 and older. It does not knowingly collect
personal information from children under 13.

## 8. Changes & contact

We will update this policy here if anything changes. Questions: contact us
at the support email shown in the Google Play Store listing (this app is
developed and maintained independently).
