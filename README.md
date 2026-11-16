# TheatreFlow Optimizer

**Project owner:** Lukyamuzi Brian

TheatreFlow Optimizer is a Node.js and Express web application for managing theatre cases and supporting operating-theatre planning with historical procedure-duration estimates.

## Main features
- User sign-in, session handling, registration and password updates
- Role-based permissions for administrators, staff and patients
- Theatre case records with patient reference, procedure, surgeon, date, theatre, priority, status and notes
- Dashboard with today's theatre plan, alerts, recent activity and case status
- Duration estimates based on historical median procedure times, with a configurable planning buffer
- Analytics and CSV/XLSX report export
- User administration, notifications, activity history and settings

## Technology
Node.js 22+, Express, SQLite (`better-sqlite3`), `bcryptjs`, Helmet, `express-rate-limit`, PDFKit and XLSX.

## Run locally
1. Install Node.js 22 or later.
2. Open a terminal in `source/app`.
3. Run `npm install` and then `npm start`.
4. Open `http://localhost:8080`.

## Initial administrator setup
For a fresh installation, set `ADMIN_EMAIL` and a strong `ADMIN_PASSWORD` environment variable before the first start if you want the application to seed an administrator account. Do not commit real credentials or patient information.

## Deployment note
This supplied build is intended for local use. Before public production deployment, configure HTTPS, secure cookies, a properly hosted database, environment-based secrets, backups and production authentication settings.

## Submission files
- `source/` — application source code
- `Project_Presentation.pptx` — project presentation
- `Final_Project_Documentation.pdf` — final project report
