# Manas College Pithoragarh – Smart Library Management System

A browser-based GitHub Pages testing version with a light navy/white/soft-blue theme.

## Updated features
- First-use screen lets you create your own password; no demo login credentials are shown.
- Log out and change-password options.
- Import/export all books, students, and transactions as a JSON backup.
- Add New Book opens in a centered modal in front of the page.
- Book fields include Accession Number, title, author, department, semester (1–6), category, Publisher / Place, ISBN, total quantity, and shelf/rack.
- Student form no longer asks for mobile number or address; semester is limited to 1–6.
- Footer: “Manas College Pithoragarh · Powered by Manshi Joshi”.
- Book issue/return, fine calculation, history, CSV exports, student ID cards and reports.

## Deploy on GitHub Pages
1. Extract this ZIP.
2. Upload `index.html` to the root of a GitHub repository. `Code.gs` is optional and only used for Google Apps Script integration.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Open the published Pages URL using HTTPS.

## Important limitations
This is a GitHub Pages testing build. Library data is stored in the current browser's `localStorage`; JSON export/import provides manual backup. The password gate is client-side only and is not secure server-side authentication. Anyone with access to the same browser profile may be able to inspect or modify browser data. Do not use it for sensitive real college records without a backend and proper authentication.

## Google Sheets (optional)
The included `Code.gs` can be deployed separately as a Google Apps Script web app for Sheets/Drive integration. Configure the API URL in `index.html` only after deploying and testing the script. The static GitHub Pages app does not connect to MySQL directly.
