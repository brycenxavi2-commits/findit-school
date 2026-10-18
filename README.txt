# FINDIT Starter Website (beginner-friendly)

## What this is
A small HTML/CSS/JavaScript prototype for the ALCHEMY '26 school startup demonstration. It includes:
- tag registration form
- found-item report form
- local coordinator dashboard
- demo tag generator and print layout
- CSV export

## Start on Windows
1. Download and extract `FINDIT_Starter.zip`.
2. Open the extracted folder.
3. Double-click `index.html`. It should open in Chrome or Edge.
4. Click **Register a tag** and register a fictional demo record, e.g. FD001 / School bag / Student A / demo@example.test.
5. Click **Report found item**, submit FD001, then open **Coordinator dashboard**.
6. Open **Make demo tags**, generate 3 tags. Internet is needed to load QR images.
7. Do not use real students' contact details in this prototype.

## Critical limitations (please read)
This is a *local demo*, not a production service:
- Data is saved in `localStorage` in the browser on this one computer.
- It does not send reports to another device.
- The dashboard has no login; anyone using this computer/browser can view demo contacts.
- QR images are generated using a third-party QR image service and require internet.
- The QR links generated while opened from `file://` will not be usable as a public phone-scanning service.

For the exhibition, this is enough to demonstrate the workflow on one computer with fictional data. To let visitors scan tags with their own phones, publish the site at a public HTTPS URL (e.g. GitHub Pages) and regenerate/test QR codes against that URL. But public hosting alone will NOT make reports sync between phones; add a secure backend or school-approved hosted form for cross-device reports before promising this as a live service.

## Safer real-world next version
For an actual school deployment:
1. Get school permission and parent/guardian consent where required.
2. Do not display owner names, phone numbers, class, or home addresses on the public page.
3. Use a school-approved form for finders; send reports to a restricted coordinator account.
4. Keep the owner register private and accessible only to authorized staff.
5. Set a data-retention rule and delete records when no longer needed.
6. Test duplicate IDs, invalid reports, QR readability, and accidental data exposure.

## Two-person team roles
- Student A: forms, QR codes, test cases and explaining the workflow.
- Student B: tag design, stall, customer survey, pricing and sales ledger.

## Suggested live demo
1. Register fictional FD001.
2. Scan/use FD001's reporting flow or manually submit FD001 in the report form.
3. Open the coordinator dashboard and show the new report.
4. Mark it returned.
5. Explain honestly that this starter's data stays in the same browser and that the next version needs secure cross-device storage.
