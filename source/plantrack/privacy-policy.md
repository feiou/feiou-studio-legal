# WeekCoach Privacy Policy

**Last updated:** September 13, 2026<br>
**Effective:** September 13, 2026

WeekCoach is operated by **Feiou Su** ("WeekCoach," "we," "us," or "our").
This Privacy Policy explains how the WeekCoach iOS and iPadOS application (the "App") handles
information. It does not cover an AI provider, website, or other third-party service that you
choose to use with the App.

WeekCoach is local-first. You can track one plan without signing in. Some information still leaves
your device for limited purposes such as anonymous authentication, privacy-conscious analytics,
purchase verification, and features you choose to enable. Cross-device content sync happens only
for a Pro user who signs in with Apple.

## 1. Information we handle

### Information you enter or import

Depending on how you use the App, this can include:

- fitness or wellness goals, preferences, constraints, and optional personal details such as age,
  sex, height, and weight;
- imported plans, plan revisions, exercise prescriptions, notes, and adjustment requests;
- completion history, set counts, timers, streaks, and metrics you record;
- Coach conversations and AI-generated plan proposals; and
- settings such as language, units, notification preferences, and AI-engine preferences.

Some of this information may reveal health or fitness information. Do not enter information you do
not want WeekCoach or a service you deliberately connect to process.

### Apple Health information

If you are a Pro user and choose to connect Apple Health, the App requests read-only access to the
specific types you approve: steps, active energy, resting heart rate, body weight, sleep, and
workouts. WeekCoach does not write to Apple Health.

Health information is queried on demand to show progress and to prepare progress or Coach context.
WeekCoach does **not** save Apple Health samples in its database, sync them to WeekCoach's cloud
database, send their values to analytics or RevenueCat, use them for advertising or marketing, or
sell them.

Your Health information can leave your device only when you direct an AI-related workflow:

- **Apple Intelligence:** processing occurs on your device through Apple's system framework.
- **Your API key:** the relevant prompt, which may include Health summaries, is sent directly to
  the compatible Chat Completions endpoint you configured. Health summaries are excluded unless you separately
  opt in to remote Health sharing in Settings; you can withdraw that permission there. The
  provider's terms and privacy policy apply.
- **Copy and paste:** a progress report may be placed on the system clipboard. It reaches another
  service only if you paste or share it there.

You control Health permissions in the Apple Health app or iOS Settings. WeekCoach cannot determine
which individual read types you denied; unavailable data simply does not appear.

### Account and device identifiers

On first launch, the App creates a random installation/account identifier and stores it in the
Keychain. It also attempts anonymous authentication with Supabase so the identifier can later be
upgraded safely for optional sync. Anonymous authentication does not upload your plans or progress.

If you choose Sign in with Apple for sync, we receive a Supabase user identifier and authentication
information needed to maintain the session. Apple may provide an email address, including a private
relay address, according to your Apple settings. We do not request your name.

### Purchase information

When WeekCoach Pro purchases are available, Apple processes the payment. RevenueCat receives a
random App User ID, App Store receipt and transaction information, product and entitlement status,
and related device or network metadata needed to offer, verify, restore, and support the purchase.
We do not receive your full payment-card details.

### Analytics and diagnostics

When analytics is configured, WeekCoach sends usage and reliability events to our own
FeiouTelemetry service at `telemetry.feioustudio.com`, using self-hosted Aptabase infrastructure.
Events include feature use, counts, permission outcomes, AI request result categories,
purchase-flow events, and sync status. They can include a random persistent installation
identifier, installation date, days since installation, session counts and durations, event
timestamps, and app, OS and device metadata. The analytics identifier is stored in local
preferences and is separate from the account identifier stored in Keychain.

App events are designed not to include plan text, prompt answers, Coach messages, Apple Health
values, manually entered metric values, API keys, Apple email addresses, or the WeekCoach account
identifier. Our hosting infrastructure receives network information, including an IP address,
to deliver requests. We do not claim that analytics are anonymous or that all infrastructure
logs exclude IP addresses. We use these data for product operation, reliability and usage
analysis, not advertising or cross-app tracking.

### Support communications

If you contact us, we process the information you provide, such as your email address, account ID,
screenshots, and message, to respond and troubleshoot. Please do not send medical records, API keys,
or other information that is not needed for support.

## 2. Where information is stored

### On your device

Plans, revisions, progress, manually entered metrics, and Coach conversations are stored in the
App's local Core Data store. Preferences and short-lived workflow state are stored in local app or
App Group storage. Partial set counts are automatically pruned after approximately 14 days.

The random account identifier, authentication session, and any AI API key you add are stored in the
Keychain. Your API key is not included in analytics, WeekCoach cloud sync, or purchase data; the App
sends it only to the endpoint you configure when making a request.

Local notifications are scheduled by iOS. WeekCoach does not operate a remote push-notification
server.

### Optional cloud sync

Content sync activates only when both conditions are met: you have Pro and you sign in with Apple.
The following data can then be stored in our Supabase project under your user ID:

- plans, plan items, source markdown, notes, status, and immutable revision history;
- completion records and manually entered item or daily metrics;
- Coach conversation titles, messages, and plan proposals; and
- record identifiers and timestamps needed for reliable synchronization and deletion.

Apple Health samples and summaries, personal prompt-builder profile settings, notification
preferences, partial set counts, and AI API keys are not synced by WeekCoach.

## 3. How we use information

We use information to:

- provide daily plan tracking, timers, progress, plan history, and Coach features;
- generate, reformat, or update plans using the AI method you select;
- provide optional cross-device sync and restore synced content;
- verify purchases and unlock Pro features;
- schedule the local reminders you enable;
- understand aggregate feature reliability and improve the App;
- prevent abuse, protect the service, troubleshoot, and provide support; and
- comply with applicable law and enforce our Terms of Use.

Where applicable law requires a legal basis, we process information as needed to perform our
contract with you, with your consent for optional permissions and features, for our legitimate
interests in operating and improving the App without overriding your rights, and to meet legal
obligations. You may withdraw consent for an optional feature, but prior lawful processing is not
undone.

## 4. When information is shared

We do not sell personal information. We do not use personal information or Apple Health information
for targeted advertising, and we do not track you across other companies' apps or websites.

We share information only as follows:

| Recipient | Purpose and information |
|---|---|
| [Apple](https://www.apple.com/legal/privacy/) | App distribution, StoreKit purchases, Sign in with Apple, HealthKit permissions, on-device Apple Intelligence, and platform services. Apple handles information under its own terms and privacy notices. |
| [Supabase](https://supabase.com/privacy) | Anonymous authentication for a stable account ID and, only after eligible Apple sign-in, storage and transport of the synced content listed above. |
| [RevenueCat](https://www.revenuecat.com/privacy) | Purchase offering, receipt validation, entitlement status, restoration, and purchase support when purchases are configured. |
| FeiouTelemetry (our self-hosted Aptabase service) | Usage and reliability events, installation/session identifiers and metadata described above, processed on our hosting infrastructure. |
| Your chosen AI provider | Prompts and context, potentially including sensitive fitness or Health summaries, sent directly to the endpoint you configure when you choose to use your API key. |
| Authorities or transaction parties | Information when reasonably necessary to comply with law, protect rights and safety, investigate fraud or abuse, or complete a merger, financing, acquisition, or transfer. We will protect information appropriately during any transfer. |

Service providers are required by contract or applicable law to protect information and process it
only for authorized purposes. A third party you independently choose, such as an AI provider you
configure or an app where you paste a report, is governed by its own terms and privacy practices.

## 5. Retention and deletion

We keep information only as long as reasonably necessary for the purposes above:

- **Local content:** stays on the device until you delete content, use **Settings → Reset local
  data**, or remove the App. Reset local data deletes local plans, completions, Coach content, and
  manually recorded metrics, but it does not by itself delete a cloud account, synced copies,
  purchase records, the account/session in Keychain, or a separately stored AI API key.
- **Keychain information:** may survive uninstalling the App, depending on iOS behavior. Clear your
  AI connection in the App before uninstalling if you want to remove the API key.
- **Synced content:** remains until you delete the relevant content or delete your account.
  Limited deletion tombstones, security logs, and backups may remain as needed to propagate a
  deletion, prevent fraud, comply with law, and complete routine backup expiration.
- **Purchase records:** Apple and RevenueCat retain transaction and entitlement records as needed
  to provide restoration, accounting, fraud prevention, and legal compliance.
- **Analytics:** installation-linked events are retained only as reasonably necessary for usage
  analysis, reliability and security. Aggregated statistics that no longer identify an installation
  may be retained longer. Clearing local app data does not itself erase previously received events;
  contact us for applicable access or deletion requests.
- **Support records:** are retained while needed to resolve the request and for reasonable legal,
  security, and operational follow-up.

You can initiate deletion of your WeekCoach account and associated content from **Settings →
Delete account**. Apple-linked accounts require a fresh Sign in with Apple confirmation so the App
can revoke that authorization before deleting the account. If the in-app flow is unavailable, email
**support@feioustudio.com** with the subject **WeekCoach account deletion** and include the account
ID shown in Settings. We may need to verify control of the account. We will complete verified
requests without undue delay and within the period required by applicable law, unless a longer
period is required or permitted. We retain only information we are legally required to keep.

Deleting a WeekCoach account does not cancel, refund, or erase an App Store purchase record. Use
Apple's purchase and refund tools for those requests.

## 6. Your choices and rights

You can:

- use the core tracker without Sign in with Apple;
- decline or revoke individual Apple Health permissions in Apple Health or iOS Settings;
- decline notifications or change them in the App and iOS Settings;
- turn off Apple Intelligence, remove your AI API key, or change the connected endpoint;
- delete individual plans or Coach conversations and reset local content in Settings; and
- request access, correction, deletion, restriction, portability, or objection where applicable.

Send privacy requests to **support@feioustudio.com**. Include your WeekCoach account ID when
the request concerns cloud or purchase-linked data. We may ask for reasonable verification. You may
also have the right to complain to your local data-protection authority. These rights are subject to
exceptions under applicable law, and we will not discriminate against you for exercising them.

## 7. Security and international processing

We use safeguards appropriate to the nature of the information, including Apple's Keychain for
credentials, encrypted network connections, access controls, and Supabase row-level authorization
for synced records. No method of storage or transmission is completely secure, so we cannot
guarantee absolute security.

Our providers may process information in countries other than the one where you live. Where
required, we and our providers use recognized transfer safeguards. Contact us for more information
about safeguards applicable to your information.

## 8. Children

The App Store listing displays WeekCoach's current content age rating. That rating describes content
suitability; it does not determine whether a person can enter a contract or consent to data
processing. We do not knowingly collect a child's personal information without the permission or
other lawful basis required where the child lives. If you believe a child provided information
without appropriate permission, contact us so we can delete it.

## 9. Changes to this policy

We may update this policy as the App, providers, or law changes. We will change the "Last updated"
date and provide additional notice in the App when a change is material. If consent is required for
a new use, we will request it before that use.

## 10. Contact

**Feiou Su**<br>
Email: **support@feioustudio.com**
