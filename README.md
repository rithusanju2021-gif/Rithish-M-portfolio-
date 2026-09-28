# Rithish M — Dynamic Portfolio Website

CS2301 Internet Programming Activity — a personal portfolio built with
HTML, CSS, JavaScript, and PHP.

## Pages
- `index.php` — Home
- `about.php` — About
- `academics.php` — Academic Details
- `projects.php` — Projects
- `achievements.php` — Achievements
- `skills.php` — Skills
- `internships.php` — Internships
- `contact.php` — Contact (dynamic form processing)
- `messages.php` — Admin login + protected message viewer (dynamic session login)

## Dynamic Features (server-side, PHP)
1. **Contact form processing** — `contact.php` validates input server-side and
   appends each submission (name, email, message, timestamp) to
   `data/messages.json`.
2. **Session-based admin login** — `messages.php` gates a data view behind a
   PHP session login. Demo credentials: `admin` / `portfolio123`.

## Running Locally
Requires PHP 8+.

```bash
php -S localhost:8000
```

Then open `http://localhost:8000/index.php` in a browser.

## Notes
- `data/messages.json` starts empty (`[]`) and is written to at runtime —
  make sure the `data/` folder is writable by the PHP process.
- Replace the placeholder GitHub/LinkedIn/email links in `php/footer.php`
  with your real profile links before publishing.
- Change `ADMIN_USER` / `ADMIN_PASS` in `messages.php` before any real deployment.
