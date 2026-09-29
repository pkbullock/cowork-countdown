# cowork-countdown
A count down to Cowork Credit renewal when credits expire before the end of the month.

## Usage

The site is a single static page (`index.html`) styled with [Tailwind CSS](https://tailwindcss.com) via the Tailwind Play CDN — no build step required.

- Open `index.html` directly in a browser, or
- Serve it locally, e.g. `python3 -m http.server 8000` and visit http://localhost:8000, or
- Publish it with GitHub Pages (Settings → Pages → deploy from the default branch root).

The countdown updates every second and targets midnight on the 1st of the next month (e.g. Oct 1, Nov 1) in the viewer's local time zone, rolling over automatically each month.
