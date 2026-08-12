# AVITAN — Privacy Policy

*Last updated: 2026-08-12*

## In one sentence

AVITAN is a **local-first** companion: almost everything you tell it stays
on your phone, in a private on-device database. It does not require an
account, does not sell data, and never shows ads. The core app is free;
optional subscriptions (AVITAN Sentience ₹399/month, AVITAN Care ₹99/month)
unlock AI chat limits and health features.

## 1. What AVITAN collects

| Data | What it is | Where it lives |
|---|---|---|
| Your chat text | The messages you type in the Chat tab | On-device database only |
| Extracted tracking data | Money, attendance, schedule, goals, sleep, water, habits, energy and screen-time logs that you confirm | On-device database only |
| Your notes (optional) | Notes you write or save from chat ("remember that…") | On-device database only |
| Your people (optional) | Names and one-line details of the close circle you choose to add (e.g. "mother, age 48") | On-device database only |
| Memory facts (optional) | Facts AVITAN remembers from what you say (e.g. where you live, your work) — with your approval, automatic or manual, and fully manageable in "What I remember" | On-device database only |
| Health readings (optional) | Blood sugar, blood pressure, heart rate, weight, steps — logged by you in chat, scanned from a lab report, or synced read-only from Google Health Connect | On-device database only |
| Lab reports (optional) | Values recognized from a photo of a lab report via on-device OCR — the photo itself is never stored or uploaded | On-device database only |
| Medications (optional) | Medication names, doses, schedules and intake adherence | On-device database only |
| Family health (optional) | Children's growth, milestones and vaccine records, and cycle/women's-health logs (period, symptoms, temperature) — entered by you for yourself or, with the in-app guardian declaration, for your own children | On-device database only |
| Notification summaries (optional) | Titles and bodies of app notifications, with names and phone numbers **redacted on-device** before storage | On-device database only |
| Usage statistics (optional) | Which apps you use and for how long (for screen-time insights) | On-device database only |
| Voice input (optional) | Your spoken words are sent to your phone's speech recognizer for transcription — AVITAN never stores or receives the audio | Processed by the Android speech service |
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

## 1c. Sharing a caregiver or doctor link (optional)

- You can create share links from the Health tab — a **caregiver link**
  (a numbers-only summary of your most recent readings, targets,
  medications, lab trends and alerts so a family member can keep an eye
  on you) and a **doctor link** (a pre-consult summary listing your
  declared conditions, targets, readings with dates and sources,
  medications, lab reports and — for children — growth, milestones and
  vaccine records). PDF copies of these summaries are generated on your
  device and only leave it when you share the file yourself.
- These links are **only created when you tap Create** — nothing is shared
  automatically, and consent is requested first.
- A link contains the summary text only (a long random token is the link's
  only credential). It is stored on our server until it expires (90 days) or
  you tap **Revoke** — revoking deletes the stored summary immediately and
  the link stops working.
- You can refresh a link at any time to update it with your latest records,
  and you can see every active link in the Health tab.

## 2. Where your data lives

- **All core data is stored in a private SQLite database on your device.**
  Nothing is uploaded to any cloud by default.
- Android may back your app data up to your Google account (Auto Backup)
  when your phone is idle; restoring to a new phone brings your data back.
- You can also export a backup file yourself from Settings → Backup & restore.

## 3. Cloud AI calls

AVITAN's chat, proactive check-ins, evening recap, morning brief and
welcome sequence use an AI model. Depending on your plan, AI access is
covered by a free welcome allowance, a free trial, a guest allowance, or
an optional subscription (AVITAN Sentience). When an AI request is made,
only the following leaves your device:

1. Your current message (or the check-in/brief text being generated).
2. A short summary of context relevant to answering it (your profile,
   recent activities, schedule, financial/attendance summaries, mood and
   health summary lines, stored memory facts, and — only for explicit
   "do you remember…" questions — a limited set of matching past records
   from your own device).

Your raw chat history is never uploaded. AI requests go through our proxy,
which does not store message content. Requests carry an anonymous install
identifier (a random ID generated on first launch, which cannot identify
you) used only to meter your free/paid usage limits. The AI provider that
generates replies is listed in §4.

Apart from AI chat, the only ways data leaves your device are the
caregiver/doctor links you create yourself (§1c), optional share exports
you make with your phone's Share menu (e.g. backup files, PDFs), and the
optional analytics digest (§1) — never anything automatic.

## 4. Third parties

| Service | Purpose | Data shared |
|---|---|---|
| Google Play | Subscription billing (AVITAN Sentience ₹399/month with ₹299 first-month intro, AVITAN Care ₹99/month, optional) | Purchase tokens (Google only, never us); Google may notify our server of subscription events to keep your license active |
| AVITAN AI proxy (our own server) | Routing AI requests and metering usage limits | Your message + context summary + anonymous install ID; no message storage |
| AVITAN share server (our own server) | Hosting caregiver/doctor links you create | The summary you chose to share, stored ≤90 days, deleted on revoke |
| DeepSeek (our AI provider) | Generating AI replies | Your message + context summary (via our proxy) |
| Google Health Connect (optional) | Read-only health data sync | Data flows from Health Connect to your device only |
| Google speech services (Android OS) | Voice input transcription and text-to-speech | Your voice/audio, processed by your device's speech service; AVITAN never stores audio |
| ML Kit / Google Play services (Android OS) | On-device OCR for lab report scans | The image is processed on your device and never uploaded |
| Sentry (optional) | Crash reporting — only if the developer enables it in the build | Anonymous device/stack-trace data, no personal data |
| Google Play Games/services (Android OS) | Standard OS services | Per Android OS policy |

## 5. Retention

- On-device data is kept until you delete it (per-entry, the in-app
  "wipe all data" button, or the memory controls) or delete the app.
- Analytics digests on our proxy are retained for 30 days and contain no
  personal data.
- Caregiver/doctor share summaries live on our server for up to 90 days
  and are deleted the moment you revoke them (§1c).
- Subscription event records on our server contain only purchase tokens
  and subscription state (active/renewed/revoked) — no personal data.
- No account, email, or phone number is ever collected or stored by us.

## 6. Your controls

- **Wipe all data**: Settings → wipe button (instant, irreversible).
- **Backup / restore**: Settings → Backup & restore (manual export/import).
- **Memory**: turn memory capture off entirely, or manage every stored
  fact in Chat → "What I remember" — correct, forget or mute each fact,
  and choose automatic or manual approval for new ones.
- **Disable capture**: turn off notification insights, screen-time, money,
  attendance, notes, health or family-health tracking at any time in
  Settings.
- **Health Connect**: connect/disconnect in the Health tab; each data type
  can be revoked individually in the Health Connect app.
- **Decline analytics**: keep "Anonymous usage analytics" off (it is off by
  default).
- **Share links**: revoke any caregiver/doctor link at any time — the
  stored summary is deleted immediately.
- **Delete the app** removes all on-device data.

## 7. Children's privacy

AVITAN is designed for users 13 and older. It does not knowingly collect
personal information from children under 13, and it is not marketed to
them. Where the app stores a child's growth or vaccine records, that data
is entered **by the child's own parent or guardian** after an explicit
in-app guardian declaration, is kept on-device, and is never collected
from children or shared except through a doctor link the parent creates
(§1c).

## 8. Changes & contact

We will update this policy here if anything changes. Questions: contact us
at the support email shown in the Google Play Store listing (this app is
developed and maintained independently).
