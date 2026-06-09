# Mathematical Physics Seminar Website

This repository contains the Jekyll/Just the Docs (Just the Class-style) source for the Perimeter Institute Mathematical Physics Seminar website:

- **Site URL:** <https://bwebste.github.io/PI-MP-Seminar>
- **Project Pages base URL:** `/PI-MP-Seminar`

## Editing the schedule

1. Open `/group-meeting.md`.
2. Update the table row for each week (date, speaker, topic, readings, notes).
3. Add or update matching reading details in `/readings.md`.

## Preview locally with Jekyll

GitHub Pages currently builds with Ruby 3.3.4, `github-pages` 232, and Jekyll 3.10.0. Use Ruby 3.3.x locally; Homebrew's latest Ruby may be too new and can cause Bundler to fall back to very old `github-pages` versions.

1. Install Ruby 3.3.4 and Bundler. With `rbenv`:
   ```bash
   brew install rbenv ruby-build
   echo 'eval "$(rbenv init - bash)"' >> ~/.bash_profile
   exec "$SHELL" -l
   rbenv install 3.3.4
   rbenv local 3.3.4
   gem install bundler:4.0.12
   ```
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
