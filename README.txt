HAVEN RESIDENCES - student dormitory website (Figma design + PHP admin)

1. Put this whole folder in C:\xampp\htdocs\   (folder name: dormitory-site)
2. Start Apache and MySQL in XAMPP.
3. Open http://localhost/dormitory-site/admin/setup.php once (safe to run again).
4. Website:  http://localhost/dormitory-site/
   Admin:    http://localhost/dormitory-site/admin/login.php   (admin / admin123)

Edit the design: open the "source-react" folder in VS Code, run:
   npm install
   npm run dev
After editing, run "npm run build", then copy everything inside source-react/dist
into this folder (do not delete the "admin" folder).
Room names/prices are at the top of source-react/src/App.tsx.
If you rename a room, also update $rooms in admin/submit_reservation.php.

Admin design: edit admin/css/style.css (colors are the variables at the top of the "v3 redesign" block).
Bootstrap is bundled in admin/vendor, so the admin works without internet.

Logo: logo.png (emblem used in the website and admin). Icons: favicon.png, favicon.ico, apple-touch-icon.png in this folder. Site name is in source-react/src/App.tsx and admin/includes/header.php.
