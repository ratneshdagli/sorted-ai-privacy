# SortMate AI – PRIVACY POLICY  
**Effective Date:** January 16, 2025  
**Last Updated:** January 16, 2025

---

## INTRODUCTION

SortMate AI ("we," "our," or "the App") is a 100% local-first productivity assistant that automatically converts messages from WhatsApp into actionable draft tasks and calendar events—all processed entirely on your device with zero cloud uploads.

Our Core Privacy Commitment:

✅ 100% On-Device Processing – All AI analysis happens locally on your phone  
✅ Zero Server Communication – Your data never leaves your device  
✅ No Data Collection – We don't collect, store, or transmit any personal data externally  
✅ Military-Grade Encryption – All local data is encrypted with AES-256-GCM  
✅ Automatic Deletion – Old messages are automatically purged (7/30/90 days or custom)  
✅ Complete Transparency – You control everything; we control nothing

This Privacy Policy explains:  
How the App processes data locally on your device  
Why we need specific permissions (Accessibility Service, Calendar)  
How your data is encrypted and automatically deleted  
What we do NOT do with your information

---

## WHAT DATA IS PROCESSED (LOCALLY ONLY)

### 2.1 WhatsApp Message Text (On-Device Only)

**What the App Does:**  
When you enable the Accessibility Service, SortMate AI reads message text directly from WhatsApp to detect tasks, events, and reminders.

**Examples of Processing:**  
"Meeting kal 3 baje" → Draft Event: "Meeting Tomorrow 3:00 PM"  
"Pay Rohit 500 for dinner" → Draft Payment Reminder: ₹500 to Rohit  
"Gym roz subah 6 baje" → Recurring Task: "Gym Daily 6:00 AM"  
"Har Monday standup 10am" → Weekly Event: "Standup Every Monday 10:00 AM"

**How It Works:**

Reading: The App uses Android's Accessibility Service API to read text content from WhatsApp messages  
Analysis: Message text is analyzed using on-device AI (no internet required)  
Extraction: Relevant information is extracted (date, time, person, amount, recurrence pattern)  
Draft Creation: A draft suggestion is created and shown to you for review  
Your Control: You must manually Confirm, Edit, or Dismiss each draft—nothing happens automatically

**Storage & Encryption:**

Message text is stored in a local encrypted database (AES-256-GCM encryption)  
Encryption keys are managed by Android Keystore (hardware-backed security)  
Field-level encryption protects message content, sender information, and metadata  
Data is inaccessible to other apps (stored in app-private directory)  
Never uploaded to any server or cloud service

**Automatic Deletion:** Messages are automatically deleted after your chosen retention period:

7 days (default)  
30 days  
90 days  
Custom (minimum 2 days)

Deletion is enforced through daily scheduled cleanup that permanently removes expired data.

---

### 2.2 Calendar Events

**What the App Does:**  
If you grant Calendar permission, SortMate AI can:

Read your existing calendar events to detect scheduling conflicts  
Write events to your calendar only when you explicitly tap "Confirm" on a draft

**Examples:**

Conflict Detection: "Meeting at 3 PM conflicts with existing Gym appointment"  
Event Creation: Tapping "Confirm" on a draft adds it to your default calendar

**Storage:**

Calendar data is accessed through Android's Calendar Provider API  
We do not store copies of your calendar events  
Calendar access is read-only until you confirm a draft

**Your Control:**

You can use the App without Calendar permission (drafts won't sync to calendar)  
Each draft requires your explicit confirmation before writing to calendar  
No auto-sync, no background changes

---

### 2.3 App Preferences (Local Only)

**What Is Stored:**

Permission status (Accessibility enabled/disabled, Calendar enabled/disabled)  
Message retention period (7/30/90 days or custom)  
Onboarding completion status  
UI preferences (language, theme settings)

**Storage Location:**

Android SharedPreferences (local device storage)  
Never transmitted to external servers

---

### 2.4 What We DO NOT Collect

The App does not collect, access, or process:

❌ Location data – No GPS or location tracking  
❌ Contacts – No access to your contact list  
❌ Photos/Media – No access to your gallery or files  
❌ Personal identifiers – No email addresses, phone numbers, or account IDs  
❌ Device identifiers – No IMEI, Android ID, or advertising IDs  
❌ Network data – No IP addresses or network requests with user data  
❌ Behavioral data – No usage analytics, screen recordings, or tracking  
❌ Keyboard input – No keystroke logging outside WhatsApp messages  
❌ Audio/Video – No microphone or camera access  
❌ Financial data – No credit card or payment information

We do not use:

❌ Analytics SDKs (Google Analytics, Firebase Analytics, Mixpanel)  
❌ Advertising SDKs (AdMob, Meta Audience Network)  
❌ Cloud services (Firebase, AWS, Google Cloud)  
❌ AI/ML APIs (OpenAI, Google Cloud AI, any external LLMs)  
❌ Crash reporting tools (Crashlytics, Sentry)  
❌ Attribution platforms (AppsFlyer, Adjust)

---

## HOW DATA IS PROCESSED

### 3.1 Core Functionality (On-Device AI)

**Processing Workflow:**  
Message Reading: Accessibility Service reads text from WhatsApp  
Local Analysis: On-device AI analyzes the text (Hinglish and English supported)  
Pattern Detection: Identifies dates ("kal," "parso"), times ("3 baje"), recurrence ("roz," "har hafte")  
Draft Generation: Creates a draft card with extracted information  
User Review: You see the draft and choose to Confirm/Edit/Dismiss  
Optional Calendar Sync: If confirmed, the event is written to your calendar

**Processing Location:**

All AI processing happens on your device's CPU/GPU  
No network requests are made for message analysis  
Works 100% offline (airplane mode compatible)

---

### 3.2 Conflict Detection

If Calendar permission is granted:

The App reads your existing calendar events  
Compares draft event times with existing appointments  
Warns you: "Meeting at 3 PM conflicts with Gym at 3 PM"

**Privacy Note:**

Calendar reading is on-demand (only when reviewing a draft)  
No calendar data is stored permanently  
No calendar data is transmitted externally

---

### 3.3 Data Retention & Auto-Deletion

**Automatic Cleanup:**

Daily scheduled task runs to delete expired messages  
Deletion is based on your chosen retention period  
Once deleted, data is permanently removed (not recoverable)

**Manual Deletion:** You can delete all data anytime:

Open Settings → Data & Privacy  
Tap "Clear All Data"  
Confirm deletion

This permanently removes:

All stored message text  
All draft cards  
All app preferences

---

## PERMISSIONS EXPLAINED

### 4.1 Accessibility Service ⚠️ (Primary Permission)

**Why We Need It:**  
Android restricts apps from reading content from other apps. To detect tasks and events from WhatsApp messages, we use the Accessibility Service API to read message text directly from WhatsApp's interface.

**What We Do:**  
✅ Read text content from WhatsApp messages  
✅ Analyze text locally using on-device AI  
✅ Create draft suggestions for you to review  
✅ Process only WhatsApp (no other apps monitored)  
✅ Respect user control (you must confirm each draft manually)

**What We Do NOT Do:**  
❌ Control WhatsApp or send messages on your behalf  
❌ Auto-confirm drafts (you must manually tap "Confirm")  
❌ Record keystrokes or passwords  
❌ Monitor banking apps, browsers, or other sensitive apps  
❌ Access WhatsApp media (photos, videos, voice notes)  
❌ Upload message text to any server or cloud service  
❌ Share data with third parties

**Scope Limitation:**  
Accessibility Service is used exclusively for reading WhatsApp message text  
We do not monitor screen content from other apps  
We do not capture UI events outside WhatsApp  
We do not use Accessibility to perform actions (clicks, gestures) on your behalf

**Compliance:**  
We comply with Google Play's Accessibility API Policy, which permits Accessibility Service usage for productivity features that help users organize information.

**Transparency:**

Permission rationale is shown before requesting access  
You can disable Accessibility anytime in Settings  
Disabling it stops new draft creation but preserves existing drafts

---

### 4.2 Calendar Permission

**Why We Need It:**  
To show your existing events for conflict detection and to write confirmed drafts to your calendar.

**What We Do:**  
✅ Read calendar events via Android's Calendar Provider API  
✅ Write events only after your explicit confirmation  
✅ Detect scheduling conflicts before creating events

**What We Do NOT Do:**  
❌ Modify existing events without your permission  
❌ Delete calendar events  
❌ Auto-sync drafts (you must confirm each one)  
❌ Access calendar data from other apps or accounts

**Your Control:**

Calendar permission is entirely optional  
You can use the App without Calendar access (drafts remain local)  
Each calendar write requires your explicit tap on "Confirm"

---

### 4.3 Storage Permission

**Why We Need It:**  
To save encrypted local data (message text, drafts, preferences).

**What We Do:**  
✅ Store data in app-private directory (inaccessible to other apps)  
✅ Encrypt all sensitive data with AES-256-GCM

---

## DATA SECURITY

### 5.1 Encryption Details

**Encryption Standard:**  
Algorithm: AES-256-GCM (Advanced Encryption Standard with Galois/Counter Mode)  
Key Management: Android Keystore (hardware-backed key storage)  
Field-Level Encryption: Message content, sender info, and metadata are individually encrypted

**Security Features:**

Authenticated encryption (prevents tampering)  
Hardware-backed keys (keys cannot be extracted)  
Per-field encryption (granular security)

**Migration:**

Existing plaintext messages are automatically migrated to encrypted format on app update  
Legacy data is securely deleted after migration

---

### 5.2 No Network Transmission

**Offline-First Architecture:**

No outbound network requests containing user data  
No background sync to cloud servers  
No API calls to external AI/ML services  
Works 100% offline (airplane mode does not affect functionality)

**Network Usage (If Any):**

App updates from Google Play 
Support links (if you tap "Contact Support")

**No Tracking:**

No analytics beacons  
No crash reporting with user data  
No advertising trackers

---

### 5.3 Access Control

**App-Private Storage:**

All data is stored in Android's app-private directory  
Inaccessible to other apps (including file managers)  
Requires root access to bypass (which voids device warranty)

**Permission-Based Access:**

Accessibility Service requires user approval  
Calendar access requires explicit permission grant  
You can revoke permissions anytime in Android Settings

---

## DATA SHARING & THIRD PARTIES

WE DO NOT SHARE YOUR DATA. PERIOD.

**No Third-Party Services:**

❌ No analytics providers (Google Analytics, Firebase, Mixpanel)  
❌ No advertising networks (AdMob, Meta Audience Network)  
❌ No cloud platforms (AWS, Google Cloud, Microsoft Azure)  
❌ No AI/ML services (OpenAI, Anthropic, Google Cloud AI)  
❌ No crash reporting tools (Crashlytics, Sentry)  
❌ No data brokers or marketing companies

**No Data Sales:**

We do not sell user data  
We do not monetize user data  
We do not share data with advertisers

**Legal Requests:** We may be legally required to disclose data if:

Compelled by court order or subpoena  
Required by law enforcement under valid jurisdiction

However: Since all data is stored locally on your device, we do not have access to your data and cannot provide it even if requested by authorities.

---

## YOUR RIGHTS & CONTROLS

### 7.1 Access & Deletion

You have complete control:

✅ Access: View all drafts within the App  
✅ Delete: Clear all data via Settings → Data & Privacy → Clear All Data  
✅ Export: No export feature (data is local-only)

**Permanent Deletion:** Clearing data permanently removes:  
All stored message text (encrypted data is overwritten)  
All draft cards  
All app settings

---

### 7.2 Permission Management

**Enable/Disable Anytime:**

Open Settings → Permissions  
Toggle WhatsApp Ingestion (Accessibility) On/Off  
Toggle Calendar Access On/Off

**Effect of Disabling:**

Stops new draft creation  
Preserves existing drafts (until you delete them or they expire)  
Does not affect calendar events already created

---

### 7.3 Retention Period Customization

**Choose Your Cleanup Schedule:**  
Settings → Data & Privacy → Message Retention Period

Options:

7 days (default, recommended)  
30 days  
90 days  
Custom (minimum 2 days, maximum unlimited)

**Daily Cleanup:**

Runs automatically every 24 hours  
Deletes messages older than your chosen retention period  
Irreversible and permanent

---

## CHILDREN'S PRIVACY

**Age Requirement:**  
SortMate AI is intended for users 13 years of age and older.

**No Children's Data Collection:**  
Since we do not collect any data (all processing is local), we inherently comply with children's privacy laws including:

COPPA (Children's Online Privacy Protection Act - USA)  
GDPR Article 8 (EU data protection for children)

**Parental Notice:** If you are a parent or guardian and believe your child under 13 is using the App, you may:

Review the App's local data (accessible only on the child's device)  
Delete all data via Settings → Clear All Data  
Uninstall the App to remove all traces

No Data to Remove: Since we do not collect, store, or transmit any data externally, there is no data on our servers to delete.

---

## INTERNATIONAL USERS

Developed In: India  
Data Residency: Your device only  
Cross-Border Transfers: Since all data remains on your device, there are no cross-border data transfers.

**GDPR Compliance (EU Users):**  
Although we are not required to comply with GDPR (as we don't process data on servers), we respect your rights:

✅ Right to Access – View all drafts in the App  
✅ Right to Erasure – Delete all data via Settings  
✅ Right to Data Portability – N/A (data is local-only)  
✅ Right to Object – Disable permissions anytime

**CCPA Compliance (California Users):**  
We do not "sell" personal information (in fact, we don't collect it). California users have:

✅ Right to Know – We tell you exactly what the App does (above)  
✅ Right to Delete – Clear all data via Settings  
✅ Right to Opt-Out of Sale – N/A (we don't sell data)

---

## CHANGES TO THIS PRIVACY POLICY

**Updates:** We may update this Privacy Policy to reflect:

App feature changes  
Legal or regulatory requirements  
User feedback

**Notification:**

Updated "Last Updated" date at the top  
In-app notification for major changes  
Continued use after changes = acceptance

**Review Regularly:** Check this policy periodically at [your website/privacy-policy-url]

---

## CONTACT US

Questions, Concerns, or Data Requests:

Email: support@sortedai.app  
Response Time: Within 48-72 hours

Mailing Address:  
SortMate AI Development Team  
[Your Street Address]  
[City, State, ZIP Code]  
India

---

## GOOGLE PLAY STORE DISCLOSURES

### 12.1 Data Safety Section Responses

For transparency, here's how we answer Google Play's Data Safety questions:

QuestionAnswerDoes your app collect or share user data?No (all processing is local)Does your app use encryption?Yes (AES-256-GCM with Keystore)Can users request data deletion?Yes (via Settings)Is data shared with third parties?NoIs data used for advertising?NoIs data used for analytics?NoDoes data leave the device?No

---

### 12.2 Accessibility Service Disclosure

Purpose: We use the Accessibility Service API solely to read message text from WhatsApp and create draft suggestions for tasks and events.

Scope: We only access:

WhatsApp message text (when explicitly enabled by user)  
Text content for AI analysis (not media, contacts, or metadata)

Processing: All text analysis happens on-device using local AI. No data is transmitted to external servers.

Compliance: We comply with Google Play's Accessibility Service Policy and use Accessibility only for its intended purpose: helping users with productivity by converting messages into actionable drafts.

User Control:

Users must explicitly enable Accessibility Service  
Clear permission rationale shown before request  
Can disable anytime in Settings

---

## TRANSPARENCY COMMITMENT

Open Development: We are committed to transparency:

📖 Technical Documentation: [Link to public docs if available]  
🛡️ Security Practices: AES-256-GCM encryption, Keystore-backed keys, daily auto-deletion  
📧 User Support: Responsive support via email

Security Researchers Welcome: We encourage responsible disclosure of security vulnerabilities.

Contact: security@sortedai.app

---

## AGREEMENT

By installing and using SortMate AI, you acknowledge that you have:

✅ Read and understood this Privacy Policy  
✅ Agreed to the data processing practices described above  
✅ Understood that all processing happens locally on your device  
✅ Understood that you can delete all data anytime

If you do not agree, please:

Do not install or use the App  
Uninstall the App if already installed

---

## SUMMARY (TL;DR)

✅ 100% Local Processing – Everything happens on your phone  
✅ Zero Data Collection – We don't collect, store, or transmit any data externally  
✅ Military-Grade Encryption – AES-256-GCM with hardware-backed keys  
✅ Automatic Deletion – Old messages deleted every 7/30/90 days  
✅ No Third Parties – No analytics, no ads, no tracking, no cloud  
✅ Complete Control – Delete all data anytime  
✅ Accessibility for Productivity Only – Reads WhatsApp messages to create drafts  
✅ Transparent & Compliant – Follows Google Play policies

Questions? Contact: support@sortedai.app

---

## END OF PRIVACY POLICY

Last Reviewed: January 16, 2025  
Version: 1.0.0
