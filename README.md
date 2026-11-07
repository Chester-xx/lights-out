<!-- Copyright (c) 2026 Lights Out. All rights reserved. Alle Rechte vorbehalten. No licence is granted; see LICENSE. -->

# **Lights Out**

### A public infrastructure damage reporter for streetlights and signals

Report a streetlight or traffic signal that is out in Gauteng, and see what has already been reported.

### **Open the app: [lightsout.org.za](https://lightsout.org.za)**

![Frontend](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FChester-xx%2Flights-out%2Fstatus%2Ffrontend.json&cacheSeconds=300)
![API](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FChester-xx%2Flights-out%2Fstatus%2Fapi.json&cacheSeconds=300)
![Database](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FChester-xx%2Flights-out%2Fstatus%2Fdatabase.json&cacheSeconds=300)
![Cloudflare](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FChester-xx%2Flights-out%2Fstatus%2Fcloudflare.json&cacheSeconds=300)

| Badge | What it checks |
|-------|----------------|
| Frontend | The website itself, lightsout.org.za |
| API | The service that receives and lists reports |
| Database | The storage behind that service |
| Cloudflare | The bot check that stops automated spam on the report form |

> **Not for emergencies.** If a fault is causing immediate danger, call the police on 10111, or 112 from a mobile phone.

## What Lights Out is

Lights Out is a public map of faulty streetlights and traffic signals in Gauteng. Choose the type of fault, mark where it is on the map or use your location, add a photo if you want to, and send it. You do not need an account.

It is for anyone in Gauteng who notices a light that is out or damaged, or a traffic signal that is not working: drivers, pedestrians, residents and neighbourhood groups.

## Why it exists

A dark street or a dead traffic signal is a safety risk, and it is rarely clear whether anyone has already reported it. Lights Out puts every report on one map so you can check first, and it groups repeat reports of the same fault instead of losing them. When you report a fault of the same type within 30 meters of an open report, yours is linked to it and the pin shows how many people have reported it.

## How a report is handled

Every report starts as **Submitted**. Moderators move it forward, and the map shows the current stage.

| Stage | Meaning |
|-------|---------|
| Submitted | Your report is received and shown on the map. |
| Acknowledged | A moderator has seen it. |
| In progress | A moderator has marked it as being worked on. |
| Resolved | A moderator has marked the fault as fixed. |

Lights Out is run independently. It is not connected to any municipality, utility or government body, and reports are not passed on to anyone today. Passing reports on to the relevant authorities automatically is planned for the future.

## What is collected

- **Your report:** the fault type, the location, an optional photo, its status and the time. No name, email, phone number or account.
- **Photos** are made smaller and re-saved on your device before they are sent, which removes hidden camera and location data. They are kept in private storage, and no screen in the app shows them today.
- **Your IP address is not stored.** It is used only to limit how fast one network can send reports, and it goes with a one-time check to Cloudflare, which tells people from bots.
- **Visit statistics:** the site uses Vercel Web Analytics and Speed Insights for anonymous visit counts and page speed. They are not tied to a person or an IP address.

## How long reports are kept

A report is deleted 6 months after it was made, or one week after it is marked Resolved, whichever comes first. If it is reopened before that week ends, the deletion is cancelled. Private weekly backups are kept for up to 90 days, so a deleted report can remain in a backup for up to that long.

## Problems and suggestions

Found a bug or have an idea? [Open an issue](https://github.com/Chester-xx/lights-out/issues/new/choose) and pick the bug report or the improvement form. Please read [CONTRIBUTING](CONTRIBUTING.md) first. For help using the app, see [SUPPORT](SUPPORT.md).

To report a faulty light or signal, use the app, not this page.

## Security

To report a security problem, use [private reporting](https://github.com/Chester-xx/lights-out/security/advisories/new) and do not post it as a public issue. Details are in [SECURITY](SECURITY.md).

## About this repository

This repository holds documentation and the public status checks only. The source code of Lights Out is not published here. Lights Out is an independent student project.

## Copyright

Copyright (c) 2026 Lights Out. All rights reserved. Alle Rechte vorbehalten. No licence is granted; see [LICENSE](LICENSE).
