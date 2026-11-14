# WellAcademy | Eng. Nasser Aboyounes

Well control assessment platform: 402-question bank, four kill sheet scenarios, review corner, exam sessions with live links, certificates, trainer dashboard and reports (PDF, Word, Excel).

(c) 2026 Eng: Nasser Aboyounes. All rights reserved.

## Files
- `index.html` the whole platform (single file)
- `firebase-config.js` your Firebase web configuration (public values)
- `firestore.rules` security rules to paste into Firebase
- `manifest.webmanifest`, `sw.js`, `icon-*.png` make the link installable as an app on phones

## Setup
1. Firebase console: create a project, add a Web app, copy the config into `firebase-config.js`.
2. Build > Firestore Database > Create database (production mode).
3. Build > Authentication > Sign-in method: enable **Anonymous** and **Email/Password**. Add one user (your trainer email and password) under Users.
4. Authentication > Settings > Authorized domains: add `nasserabounis-ops.github.io`.
5. Firestore > Rules: paste `firestore.rules`, replace `REPLACE_WITH_TRAINER_EMAIL` with your trainer email, Publish.
6. Commit `firebase-config.js`. The public link is `https://nasserabounis-ops.github.io/WellAcademy/`.
