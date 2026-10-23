# AMORA — Enterprise AI Infrastructure

A React + Vite website based on the supplied AMORA concept. The supplied website copy is preserved in `src/data/websiteContent.js`.

## Requirements
- Node.js 18+ (recommended)
- npm

## Run the website
```bash
npm install
npm run dev
```
Open the local address Vite prints (normally http://localhost:5173).

## Build for production
```bash
npm run build
npm run preview
```

## Optional demo/audit form API
In a second terminal:
```bash
npm run server
```
The API runs at http://localhost:5000. Copy `.env.example` to `.env` and replace `SMTP_PASS` with an app password generated in the Google account's security settings (do not use the normal account password). Once SMTP is configured, demo form inquiries and messages submitted in the chatbot are emailed to `amora.aitech@gmail.com`; the form sender's address is set as Reply-To. Never commit `.env` or expose SMTP credentials in frontend code. Without SMTP configuration, the API returns an error rather than pretending the message was sent. Publish the site to a stable public HTTPS URL before creating a website QR code; a QR to localhost will not work for visitors.

## Notes
- ROI calculator is an illustrative estimate using user-entered values. It does not change the supplied AMORA copy.
- The website preserves the provided security and cost claims as supplied. Validate all claims against the actual deployment and legal/compliance requirements before publishing.
