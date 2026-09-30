# cowork-countdown
A count down to Cowork Credit renewal when credits expire before the end of the month.

## Usage

The site is a single static page (`index.html`) styled with [Tailwind CSS](https://tailwindcss.com) via the Tailwind Play CDN — no build step required.

- Open `index.html` directly in a browser, or
- Serve it locally, e.g. `python3 -m http.server 8000` and visit http://localhost:8000, or
- Publish it with GitHub Pages (Settings → Pages → deploy from the default branch root).

The countdown updates every second and targets midnight on the 1st of the next month (e.g. Oct 1, Nov 1) in the viewer's local time zone, rolling over automatically each month.

## Positivity features

- While counting down, one of five upbeat "you're winning the race" messages is picked at random on page load and shown below the progress bar.
- On renewal day (the 1st of the month) the countdown and progress bar are hidden and replaced by a colourful confetti celebration. The countdown to the next renewal resumes on the 2nd.
- To preview the celebration on any day, add `?renewal=true` to the URL (e.g. http://localhost:8000/?renewal=true).
