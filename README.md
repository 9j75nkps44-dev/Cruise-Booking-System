IVY CRUISE DESK — README
Version 1.0

OVERVIEW
Ivy Cruise Desk is a personal cruise sales and booking follow-up web app for Ivy. It helps organize customer inquiries, quotations, booking statuses, sailing dates, payment deadlines, and follow-up activities in one place.

FEATURES
- Dashboard with active customers, follow-ups due, pending payments, and upcoming sailings
- Customer and booking records
- Cruise line, ship, itinerary, sailing date, booking reference, and guest details
- Sales pipeline statuses:
  New Lead
  Quotation in Progress
  Quotation Sent
  Follow-Up Required
  Pending Confirmation
  Awaiting Payment
  Booked / Confirmed
  Cancelled / Lost
- Follow-up dates, reasons, contact history, and notes
- Sailing tracker and final payment due dates
- Import existing records from CSV or Excel (.xlsx / .xls)
- Export bookings as CSV and create a JSON backup
- Responsive layout for iPad and desktop browsers

FILES
- index.html: The main web app. Upload this file to your web host or GitHub repository.
- README.txt: This guide.

HOW TO USE
1. Open the deployed app in a supported browser.
2. Choose Add booking to enter a customer manually, or open Import from Excel to bring in an existing spreadsheet.
3. For Excel import, choose the file, select Preview import, review the sample rows, then select Import records.
4. Open Customers & Bookings to search and edit records.
5. Use Follow-ups to log calls, record outcomes, and schedule the next contact.
6. Use Sailing Tracker to review departure dates and payment deadlines.
7. Export CSV or download a JSON backup regularly.

EXCEL IMPORT
The import tool expects a header row. Recommended column names include:
Customer Name, Phone, Email, Preferred Contact, Cruise Line, Ship, Destination, Sailing Date, Duration / Guests, Booking Ref, Status, Sales Owner, Quote Value, Currency, Deposit Due, Balance Due, Final Payment Due, Last Contact, Follow-up Date, Follow-up Reason, Notes.

Column names may vary, but using the suggested headings is recommended. CSV import is built in. Excel (.xlsx / .xls) import loads an Excel-reading library from a CDN, so an internet connection is required for those file types.

When a booking reference matches an existing record, the importer updates that record. Rows without a matching booking reference are added as new records. Review your spreadsheet and preview carefully before importing to avoid duplicates.

DATA STORAGE AND PRIVACY
Version 1 stores records in browser local storage on the device and browser where the app is used. It does not provide automatic cloud sync or shared access between devices. Browser data clearing, device loss, or some browser settings may remove local records. Export backups regularly and store them securely.

This version processes selected import files in the browser. Do not treat it as a centrally managed or enterprise-secure CRM. Before storing sensitive customer information, use a properly secured hosting and database setup with authentication, access controls, backups, and any required company approval.

INSTALLATION / HOSTING
For everyday use, host index.html on a trusted HTTPS static web host such as GitHub Pages or Cloudflare Pages:
1. Create a repository or project for the app.
2. Upload index.html (and this README file if desired).
3. Enable the host's static-site publishing feature.
4. Open the HTTPS URL in Safari on the iPad.
5. In Safari, use Share > Add to Home Screen if that option is available.

A static deployment alone does not add cloud database sync, user accounts, automatic reminders, email/SMS sending, or a cruise line booking-platform integration.

IMPORTANT NOTES
- Dashboard numbers are calculated from the records entered or imported; no demo customer records are included by default.
- Payment totals may contain multiple currencies. The app does not convert currencies, so do not treat a combined total across currencies as one financial amount.
- Keep booking status, balance, sailing date, and follow-up date up to date.
- Verify imported dates and statuses after import.
- CSV files can be opened in Excel, but formatting may differ from a native Excel workbook.

NEXT POSSIBLE IMPROVEMENTS
- Installable Progressive Web App (PWA) support and offline caching
- Cloud database and secure login
- Automatic reminders and notifications
- Excel (.xlsx) export
- Multi-agent access and sales performance reporting
- Integration with approved cruise line booking systems

END OF README
