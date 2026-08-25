Baghwan Fruit Suppliers - Billing App

Setup:
1. Copy `js/firebase-config.example.js` to `js/firebase-config.js` and fill your Firebase config.
	- Create a Firebase project, enable Firestore (native mode), Storage, and Authentication (Email/Password).
2. Serve `index.html` (use `firebase deploy` or a static server).

Quick Test Steps:
1. Open `index.html` in browser after providing `js/firebase-config.js`.
2. Create an account via `login.html` (Email/Password).
3. On Billing page, fill sample data and click `SUBMIT BILL`.
4. Check Firestore `bills` collection, `customers`, and `auditLogs` for created documents.

Notes:
- This project uses Firebase (Auth required for secure reads/writes). Fill config before use.
- Marathi number-to-words converter included (basic implementation). It uses Indian numbering but is an approximate linguistic helper.
- Drafts are auto-saved to localStorage when offline or between sessions. Drafts sync when you sign in and submit.
- Do NOT commit `js/firebase-config.js` with real credentials to public repositories.

