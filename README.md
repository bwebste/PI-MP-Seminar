# Mathematical Physics Seminar Website

This repository contains the Jekyll/Just the Docs (Just the Class-style) source for the Perimeter Institute Mathematical Physics Seminar website:

- **Site URL:** <https://bwebste.github.io/PI-MP-Seminar>
- **Project Pages base URL:** `/PI-MP-Seminar`

## Editing the schedule

1. Open `/group-meeting.md`.
2. Update the table row for each week (date, speaker, topic, readings, notes).
3. Add or update matching reading details in `/readings.md`.

## Preview locally with Jekyll

1. Install Ruby and Bundler.
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Start the local server:
   ```bash
   bundle exec jekyll serve
   ```
4. Open <http://127.0.0.1:4000/PI-MP-Seminar/>.

## GitHub Pages deployment

This is configured as a **GitHub Pages project site** using:

- `url: "https://bwebste.github.io"`
- `baseurl: "/PI-MP-Seminar"`
- `remote_theme: just-the-docs/just-the-docs`

GitHub Pages builds and publishes from this repository using Jekyll-compatible settings in `/_config.yml`.
