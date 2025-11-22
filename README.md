# Ecommerce Project

**Full-stack E‑commerce Web Application**

A complete e-commerce web application with user authentication, product management, cart system, and an admin dashboard.

---

## Quick description

This is a full-stack e-commerce project featuring user registration, login, product browsing, cart management, and an admin panel for product CRUD operations. Built to learn and demonstrate web development concepts using PHP, MySQL, and plain HTML/CSS (modify stack details if needed).

---

## Features

* User signup / login / logout (session-based)
* Product listing and product detail pages
* Add to cart / remove from cart
* Simple checkout flow (mock)
* Admin dashboard: login, add / edit / delete products
* Responsive layout for desktop and mobile

---

## Tech stack

* Frontend: HTML, CSS, (basic JS)
* Backend: PHP
* Database: MySQL / MariaDB
* Server: (deployable to shared PHP hosts or Docker)

> Edit this section if your project uses Node/Express/React or other tech.

---

## Screenshot

![project screenshot](/mnt/data/Screenshot 2025-11-22 110613.png)

---

## Folder structure (example)

```
/ecommerce-project
  /admin
  /images
  /pages
  /includes
  index.php
  README.md
```

---

## Requirements (local)

* PHP 7.4+ (or PHP 8)
* MySQL / MariaDB
* A local development environment like XAMPP / WAMP / Laragon
* Git (for version control)

---

## Setup — run locally (XAMPP / WAMP)

1. Copy the project folder into your web server's `htdocs` (XAMPP) or `www` (WAMP) folder. Example:

   * `C:\xampp\htdocs\ecommerce-project`
2. Start Apache and MySQL from XAMPP/WAMP control panel.
3. Create a database in phpMyAdmin (for example: `ecommerce_db`).
4. Import the SQL if provided (or create tables manually) — see `00_documentation.md` for DB schema.
5. Update DB config in `includes/db.php` (set DB name/user/password):

```php
// example: includes/db.php
$host = 'localhost';
$user = 'root';
$pass = '';
$db   = 'ecommerce_db';
```

6. Open in browser: `http://localhost/ecommerce-project/` and test flows.

---

## .env / config example (safe to include as `.env.example`)

```
DB_HOST=localhost
DB_USER=root
DB_PASS=
DB_NAME=ecommerce_db
```

> **Do not** commit real credentials. Keep `.env` or `includes/db.php` with placeholders and add `.gitignore` to ignore real `.env`.

---

## How to push changes

```bash
git add .
git commit -m "your message"
git push
```

---

## How to show this project in interviews

1. Open the live site (or `http://localhost/...`) and perform these actions: signup → login → add item to cart → view cart → mock checkout.
2. Open `includes/db.php` to explain DB connection and show table structure in phpMyAdmin.
3. Open GitHub repo to show commit history and README.
4. Explain the authentication flow, where sessions are created, and how admin actions work.

Suggested 60–90 second script (copy-paste in interview):

> "This is a full-stack e-commerce application I built and configured. The app supports user registration and login, product listing, a cart system and an admin dashboard for managing products. I implemented session-based authentication, connected the app to a MySQL database, and structured the code to separate admin and customer flows. I can demo the signup, add-to-cart, and admin add-product flows now."

---

## Deployment notes

* For PHP projects you can use shared hosts (InfinityFree, 000WebHost) or VPS.
* Update DB credentials on the server and import DB.
* If you later migrate to a Node/React stack, consider Vercel + Render or Railway.

---

## Troubleshooting

* If pages show blank: enable PHP error reporting in `php.ini` or add at top of PHP files:

```php
ini_set('display_errors', 1);
error_reporting(E_ALL);
```

* If DB connection fails: check host/user/password and that MySQL is running.

---

## License

Add a license file if you want (MIT recommended for portfolios):
`LICENSE` (MIT)

---

## Author

**Harshitha Mahesh** — built, configured, and deployed.

---

If you want, I can also:

* Generate a `.gitignore` and `.env.example` for you.
* Produce a short `CONTRIBUTING.md` or `CHANGELOG.md`.
* Create a README tailored for a different tech stack (React/Node/MongoDB).

Tell me what you want next.
