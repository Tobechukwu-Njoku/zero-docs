---
layout: default
title: Databasus - Privacy Policy
last_updated: 2026-10-24
---

This policy explains what data Zero-Technologies' self-hosted instance of Databasus ("the Service") uses, why, and what rights you have. The data controller is {{ site.controller }} ("we", "us"). Contact: [{{ site.contact_email }}](mailto:{{ site.contact_email }}).

The Service is an internal backup tool. Its only user is the Zero-Technologies administrator.

## 1. Data we collect

| Data | Why |
|---|---|
| The administrator's account: email address, name and a hashed password, or the email address and name from Google sign-in | To sign in to the Service |
| Google OAuth tokens for the connected Google Drive account | To upload, list and delete backup files in that Drive |
| Database connection details and schedules | To make the backups |
| Backup files | To restore Zero-Technologies services after a failure |
| Backup logs and alert history | To show whether backups worked and to send alerts |

**Backups contain the data of the services they protect.** For example, a backup of the Zero-Technologies Sign-in database contains the account data described in the [Sign-in Privacy Policy](/sign-in/privacy/). Backups are copies kept only for restoring those services. We do not use them for anything else.

## 2. Google user data

When a Google account is connected, the Service requests:

- **`https://www.googleapis.com/auth/drive.file`**, to create, read and delete only the files the Service itself uploads. The Service cannot see, open or change any other file in that Google Drive.
- If Google sign-in is turned on, the account's **email address and basic profile** (name), to identify the administrator.

The Service uses this data only to store and manage its own backup files and to sign the administrator in. It does not use Google user data for advertising, does not sell it, and does not transfer it to anyone else, except to Google itself to perform those actions. No human reads it, except the administrator managing their own backups.

Databasus's use and transfer of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

## 3. Legal basis

- The administrator's own account and Google data: to provide the Service the administrator set up for themselves (UK GDPR Article 6(1)(b)).
- Personal data inside backups: our legitimate interest in being able to recover our services and the accounts of their users after a failure (UK GDPR Article 6(1)(f)).

## 4. How long we keep it

- Backups are deleted automatically by each backup's retention rule (a set number of copies or days).
- Google OAuth tokens are kept until the Google account is disconnected from the Service or Google access is revoked.
- Account data and logs are kept while the Service is in use.

## 5. Who we share it with

We do not sell data or share it for advertising. It is processed by:

- **Google**, only when Google Drive storage or Google sign-in is used ([Google Privacy Policy](https://policies.google.com/privacy))
- **Google (Gmail)**, which delivers alert emails
- **Cloudflare**, which carries traffic to the Service's web address ([Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/))
- Our own self-hosted servers in the United Kingdom

## 6. Security

The Service runs on servers we control. Its web interface is reachable only over HTTPS at `sv01-databasus.zero-technologies.co.uk` and requires the administrator's sign-in. Access is limited to the administrator. Google tokens and database passwords are stored on our servers only.

## 7. Your rights

Under UK data protection law, you can ask us to:

- Give you a copy of your data
- Correct or delete your data
- Restrict or object to how we use it

If you have an account with a Zero-Technologies service, your data may also be in that service's backups until they expire. Email [{{ site.contact_email }}](mailto:{{ site.contact_email }}). We will reply within one month.

If you are unhappy with how we handle your data, you can complain to the [Information Commissioner's Office (ICO)](https://ico.org.uk/make-a-complaint/).

## 8. Changes

We may update this policy. The "Last updated" date above shows when it last changed.
