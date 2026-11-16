# AUTOVEX ULTIMATE — starter project

A responsive automotive marketplace front-end with a PHP/MySQL schema starter.

## Included
- Responsive AUTOVEX landing page and vehicle marketplace.
- Sample vehicle cards with search, type/price filters and sorting.
- Save/favourite buttons stored in browser localStorage.
- Dark/light theme toggle.
- Login and registration screens with Google and Apple sign-in entry points.
- Seller listing form preview.
- MySQL schema for users, vehicle listings, saved vehicles, conversations and messages.
- Role types for buyers, sellers, dealers, service providers and administrators.

## Run the front-end
You can open `index.html` directly in a browser, or place the folder inside `C:\\xampp\\htdocs\\AUTOVEX-ULTIMATE` and visit `http://localhost/AUTOVEX-ULTIMATE/`.

## Set up the database (XAMPP)
1. Start Apache and MySQL.
2. Open phpMyAdmin.
3. Import `backend/database.sql`.
4. Copy `backend/config.example.php` to `backend/config.php`.
5. Add your local database credentials to `config.php`.

## Important: what is demo-only
This ZIP is a front-end and database starter, not a production marketplace. The login/register buttons, Google/Apple buttons, phone field, listing preview, and sample inventory are interface demonstrations. They do not create accounts, send SMS, verify email, authenticate with Google/Apple, publish database listings, process payments, or provide live chat yet.

To activate real Google sign-in, configure an OAuth 2.0 client and secure callback endpoint. For Apple, configure Sign in with Apple and its service identifiers/keys. For phone verification, integrate a reputable SMS/OTP provider. Keep provider secrets on the server; never ask users for their Google or Apple passwords. Use HTTPS, CSRF protection, server-side validation, rate limits, secure session cookies, upload validation, authorization checks, backups and privacy/consumer-law review before launch.

## Suggested next development milestone
Build the PHP API endpoints for account registration/login, email verification, SMS OTP, listing upload/publication, seller dashboard and authenticated messaging. Then connect the UI to those endpoints and test each flow.
