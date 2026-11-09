# Kids Empire Construction Checklist PWA

## Deploy
Upload the contents of this folder to any HTTPS static web host. The files must remain together. Open `index.html` through the site URL.

Examples of suitable hosting: GitHub Pages, Cloudflare Pages, Netlify, Vercel, or an existing company HTTPS web server. No server-side code or database is required for this version.

## iPhone / iPad installation
1. Open the HTTPS URL in Safari.
2. Tap Share.
3. Tap **Add to Home Screen**.
4. Launch **KE Checklist** from the Home Screen.
5. After the first successful online load, the app shell works offline.

## Data behavior
- Current inspection data is stored locally on that browser/device.
- **Save Inspection** explicitly marks the current state saved locally.
- **Export Backup** downloads a JSON backup for transfer/archive.
- **Import Backup** restores a JSON backup.
- Filters require every checklist item to have a response; partial inspections can still be saved.
- Section I uses Yes/No + Notes. Sections A-H use Complete / Not Started / whole-number % Complete + Notes.

## Important
This first PWA is device-local. It does not synchronize inspections between team members or devices. Team/cloud synchronization would require a hosted backend or shared data service.
