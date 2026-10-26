BARANGAYCARE (Node.js + SQLite version, works with SQLiteStudio)

SETUP (Windows)
1. Install Node.js 22.5 or newer (the LTS version) from https://nodejs.org  (check with:  node -v)
2. Unzip this folder anywhere, e.g. Documents\barangaycare
3. Double-click  start.bat   (or open a terminal in the folder and run:  node server.js)
4. Open http://localhost:3000  in your browser. Do NOT double-click the html files.
   Keep the black window open while using the site. Press Ctrl+C in it to stop.

THE DATABASE (SQLiteStudio)
- The database file is  database\barangaycare.db
- In SQLiteStudio:  Database > Add a database > pick that file > Connect.
  Tables: users, residents, appointments, emergencies.
- The table design is also in  database\schema.sql
- You can view and edit data in SQLiteStudio while the site runs. Click "Commit" after editing,
  and refresh the website to see the changes.
- To reset everything: stop the server, delete database\barangaycare.db, start again
  (a fresh database with the demo data is created automatically).

DEMO LOGINS (passwords are stored hashed, so you will not see them in the database)
  Administrator: admin / Admin123!
  Resident:      resident / User123!

FILES
  server.js     the server + API (no npm install needed)
  database/     barangaycare.db + schema.sql
  css/ js/      front end
