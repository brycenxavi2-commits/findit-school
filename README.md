# FINDIT Pro Plus — Enhanced School Recovery Prototype

## Features
- Responsive dashboard and quick actions
- Unique FINDIT tag IDs
- QR code preview, single-label print and QR image open/download
- Bulk QR-label print sheet
- Inventory search and category/status filters
- Quick lookup by pasted/scanned FINDIT ID (`FINDIT|FND-...` is accepted)
- Found-item desk, return tracking, and status changes
- Edit item details and delete records
- Recent activity log and activity-log JSON export
- Full inventory JSON backup/restore and CSV export
- Demo sample records and clear-local-data control
- Form validation, escaped user content, and localStorage error handling

## Run
Extract the ZIP and open `FINDIT_Pro/index.html` in a modern browser. QR images require an internet connection.

## Publish
Upload `index.html` to the repository branch/folder configured for GitHub Pages, commit the changes, then refresh the published website (Ctrl+F5).

## Limitations
This is still a static front-end prototype. Data lives in the current browser's localStorage and does not sync to other devices. The QR encodes only `FINDIT|TAG-ID`; it does not open a cloud-hosted item record on a separate device. QR image creation uses a third-party online QR image service. There is no staff authentication or shared database. For real school deployment, add a secure backend/database, access controls, and school-approved privacy handling.

## Verification performed
- Extracted inline JavaScript and ran `node --check` successfully.
- This syntax check does not replace end-to-end browser testing on the target school's devices.
