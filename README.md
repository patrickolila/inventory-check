# Inventory Check

A web app that compares an expected inventory PDF against a physical pack sheet scan and reports discrepancies.

**Live app:** `https://<your-username>.github.io/inventory-check/`

## How it works

1. Enter your Anthropic API key (saved in browser, never leaves your device except to call Claude)
2. Upload the expected PDF (from WhatsApp) and the actual sheet (scanned)
3. The app identifies the correct date column, asks you to confirm
4. It reads all pages and returns a discrepancy report
5. One-click copy of a WhatsApp-ready message

## Setup (GitHub Pages)

1. Create a new repository on GitHub called `inventory-check`
2. Upload `index.html` to the repository
3. Go to **Settings → Pages → Source** and select `main` branch
4. Your app will be live at `https://<your-username>.github.io/inventory-check/`

## Requirements

- An Anthropic API key with credits ([console.anthropic.com](https://console.anthropic.com))
- A modern browser (Chrome, Firefox, Safari, Edge)
- No server, no backend, no install needed

## Security note

Your API key is stored in your browser's localStorage for convenience. It is only ever sent directly to Anthropic's API. If you share the device with untrusted people, clear localStorage or use a private/incognito window.

## Cost

Each run costs roughly $0.05–$0.15 in API credits depending on PDF size.
