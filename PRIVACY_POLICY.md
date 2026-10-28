# Privacy Policy — WhatsApp Sorting Chrome Extension

**Last updated:** October 28, 2026

## What this extension does

WhatsApp Sorting is an internal productivity tool used by our customer service team on WhatsApp Web (web.whatsapp.com). It provides:

- Live translation of incoming customer messages
- Voice note transcription (speech to text)
- Contact extraction and sync to a private Google Sheet

This extension is **not affiliated with, endorsed by, or connected to WhatsApp or Meta Platforms, Inc.**

## What data is collected

### Data processed locally (never leaves your browser)

- Message text displayed on WhatsApp Web (read-only, used for translation)
- Voice note audio from WhatsApp Web (read from WhatsApp's in-memory data, used for transcription)
- Contact names and phone numbers visible in WhatsApp Web chats

### Data sent to external services

| Data | Sent to | Purpose | Retention by the service |
|---|---|---|---|
| Message text (incoming only) | Google Translate (translate.googleapis.com), Google clients5, or MyMemory (api.mymemory.translated.net) | Translation into the agent's chosen language | Per each service's standard privacy policy |
| Voice note audio | Groq (api.groq.com) | Speech-to-text transcription | Per Groq's privacy policy (https://groq.com/privacy-policy/) |
| Contact name, phone number, status | A private Google Apps Script endpoint (Google Sheets) | Syncing contacts to a team spreadsheet | Stored in the team's own Google Sheet |

### Data NOT collected

- We do **not** collect, store or transmit any data to our own servers.
- We do **not** use analytics, tracking pixels, cookies or advertising.
- We do **not** sell, rent or share any data with third parties for advertising or marketing.
- We do **not** store message content, voice recordings or transcripts after the browser tab is closed.
- We do **not** access WhatsApp chats other than the one currently open on screen.

## Permissions used

| Permission | Why it's needed |
|---|---|
| `storage` | Saves toggle states and agent name locally in the browser |
| `activeTab` | Reads the currently open WhatsApp Web tab |
| `scripting` | Injects the translation and extraction script into WhatsApp Web |
| `alarms` | Triggers automatic contact sync every 8 hours |
| Host permission: `https://web.whatsapp.com/*` | The only website this extension runs on |
| Host permissions: translation and transcription APIs | Sends text or audio to the services listed above |

## Data security

- All communication with external APIs uses HTTPS encryption.
- The Groq API key is stored locally in the extension's background script file. It is not transmitted anywhere other than to Groq's API.
- The Google Sheet webhook URL is stored in the extension's background script file.

## Who controls this extension

This extension is developed and maintained internally by our team for our own use. It is not a public product.

For questions about this privacy policy, contact the extension maintainer within the team.

## Changes to this policy

We may update this privacy policy when the extension's functionality changes. The "Last updated" date at the top reflects the most recent revision.
