# Kids Empire Construction Checklist PWA v6

## Workflow
- Launching the Home Screen icon opens app navigation.
- **Start New Inspection** creates a separate inspection record and begins continuous local autosave.
- **Load Saved Inspection** lists all inspections currently stored on that device.
- **Share Inspection** is available at the bottom of the inspection form. It will not generate reports until every checklist item has a response.
- A successful share attempt generates two PDFs: Complete Items and Open Items & Site Conditions.
- After the share sheet returns, the app displays **Confirm Report Share**, **Close Report**, and **Return to Inspection**.
- **Confirm Report Share** is the only workflow action that deletes that inspection. It requires a second deletion confirmation.
- **Close Report** returns Home and retains the inspection.
- **Return to Inspection** retains and reopens the current inspection so it can be edited or shared again.

## Storage
Inspection data is stored locally in browser/PWA storage on the device. Multiple inspections may coexist. PDFs are generated on demand and are not retained by the app. Clearing browser/site data or removing the PWA may remove locally stored inspections.

## Deployment
Upload all files and the `icons` folder to the repository root used by GitHub Pages. The service-worker cache name is `ke-checklist-v6` so installed PWAs receive the updated app shell.

## v7 icon update
- Final Home Screen icon uses the approved KE/checkmark design.
- Includes 180x180, 192x192, and 512x512 icon assets.
- Service-worker cache bumped to `ke-checklist-v7` so updated icon assets are fetched.
