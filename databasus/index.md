---
layout: default
title: Databasus
---

Databasus is the database backup service that Zero-Technologies runs on its own servers. It makes scheduled backups of the databases behind Zero-Technologies services and stores them on our own disks and, optionally, in a Google Drive account we own. It also sends alerts about backups by email.

It is an internal tool used only by the Zero-Technologies administrator. It is not offered to the public, and you cannot sign up for it.

## Google Drive and Google sign-in

When a Google account is connected to Databasus:

- Databasus asks Google only for the **`drive.file`** permission. It can create, read and delete the backup files it uploads itself, and **cannot see any other file** in that Google Drive.
- If Google sign-in is turned on, Databasus receives the account's email address and name to identify the administrator.

To disconnect it, remove Databasus's access under **Google Account > Security > Third-party apps with account access**.

## Policies

- [Terms of Service](/databasus/terms/)
- [Privacy Policy](/databasus/privacy/)
