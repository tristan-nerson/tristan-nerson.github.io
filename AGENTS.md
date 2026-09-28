# Site editing notes

This repository is Tristan Nerson's public academic site, built with al-folio/Jekyll. Edit content under `_pages/`, `_bibliography/`, and `_data/`. Keep the source and public pages free of private contact details and unpublished project details. Peer-review entries list journals and counts, never manuscript titles.

The site uses the `al_folio_core` theme gem. Do not add local `_layouts/`, `_includes/`, `_sass/`, `_scripts/`, or a separate CSS build pipeline. Keep `Gemfile` and `_config.yml` aligned when changing plugins.

Before publishing, run `npm run lint:prettier` when Node dependencies are installed. For substantial changes, open a pull request and verify the **Deploy site** build; merging to `main` publishes the site through GitHub Actions. GitHub Pages must use **Source: GitHub Actions**.
