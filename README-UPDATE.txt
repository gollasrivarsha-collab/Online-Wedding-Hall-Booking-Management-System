SRIVARSHA WEDDING - FRONT-END REDESIGN
=====================================
This ZIP contains a replacement public folder with 8 customer pages and 5 admin pages.

INSTALL:
1. Stop the Node server in VS Code using Ctrl+C.
2. Back up your existing project/public folder.
3. Extract this ZIP.
4. Copy the CONTENTS of the included public folder into your existing project's public folder.
5. Choose Replace files if prompted.
6. Do NOT replace server.js, .env, package.json, database files, or node_modules.
7. Run npm start from the folder containing package.json.
8. Open http://localhost:3000

PAGES:
index.html, halls.html, booking.html, about.html, login.html, register.html,
my-bookings.html, contact.html, admin/login.html, admin/dashboard.html,
admin/bookings.html, admin/customers.html, admin/halls.html.

IMPORTANT:
- Wedding hall photos use remote images from images.unsplash.com, so internet access is needed to display them.
- Hall cards include sample fallback details if /api/halls fails. Sample hall details are for display only and are not inserted into MySQL.
- Existing server.js expects the halls table to contain an is_available column. The user's current database previously reported "Unknown column is_available". The front end cannot fix that SQL mismatch. Before booking/hall loading works fully, the database and server query must be aligned. Back up the database before making schema changes.
- Contact page is an enquiry guide, not a message-saving form.
- Admin login requires ADMIN_EMAIL and ADMIN_PASSWORD in .env.
- This is a local learning project, not production-ready security.
