# Tristan Nerson's academic website

Source for [tristan-nerson.github.io](https://tristan-nerson.github.io/). The site uses the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme and publishes through GitHub Actions.

## Update the site

- Edit the text in `_pages/`: `about.md` is the home page; `research.md`, `publications.md`, `teaching.md`, `talks.md`, and `cv.md` are the other pages.
- Edit `_bibliography/papers.bib` for publications. Keep BibTeX commas between fields. `selected = {true}` shows a paper on the home page. Do not include confidential manuscript details.
- Edit `_data/socials.yml` for public contact links.
- Keep personal photos in `assets/img/`; the research video is in `assets/video/`.

Commit changes to `main` to publish them. The **Deploy site** workflow builds Jekyll and uploads the site to GitHub Pages. Check its result under **Actions**. The **Prettier code formatter** and **Check for broken links on site** workflows are additional checks. GitHub Pages should be configured with **Source: GitHub Actions** in **Settings → Pages**.

For a local formatting check, run `npm ci && npm run lint:prettier`. A local Jekyll build requires Ruby and the gems in `Gemfile.lock`: `bundle install && bundle exec jekyll build`.
