# Kids Empire Construction Checklist PWA

## Deploy
Upload the contents of this folder to the GitHub Pages repository root, replacing the existing files. Keep the `icons` folder in the repository.

## Field workflow
1. Launch the bookmarked / Home Screen PWA.
2. Complete the inspection. Sections A-H use Complete, Not Started, or whole-number % Complete. Section I uses Yes/No.
3. Tap **Share Inspection**.
4. The app creates two small PDFs and opens the device share sheet when file sharing is supported:
   - **Complete Items Report** — all completed A-H items, including their notes.
   - **Open Items & Site Conditions Report** — Not Started items, 1-99% items, all Section I Yes/No items, and notes from completed items.
5. Completed-item notes in the Open Items report are abbreviated as `Completed Item Note - G7 POS Systems: [note]` rather than repeating the full checklist question.

The user can choose Mail, Messages, Outlook, AirDrop, Files, or another available share destination. If the browser cannot share files, the app falls back to downloading both PDFs.

## Data behavior
Inspection work is continuously stored locally on the device so a page refresh does not erase progress. There is no import/export backup workflow and no New Blank Inspection control. Start a new inspection by launching the deployed checklist from the bookmark/Home Screen after the prior inspection workflow is complete.

## Offline behavior
After a successful online load, the app shell is cached by the service worker for offline use.
