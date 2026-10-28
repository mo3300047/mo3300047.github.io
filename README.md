# Liyuan Guo’s personal website

Personal website published at https://mo3300047.github.io/ using Jekyll and GitHub Pages.

## Content and structure

- `_pages/`: homepage, experience, projects, education, skills, publications, sitemap, and 404 page.
- `_data/navigation.yml`: main navigation.
- `_config.yml`: author details and production settings.
- `_layouts/`, `_includes/`, `_sass/`, and `assets/`: shared theme templates, styles, scripts, and fonts.
- `images/`: portrait and site icon.

Each public route has one source page. For example, `/work/` comes from `_pages/work.md`.
Generated HTML in `_site/` is ignored and must not be committed.

## Local preview

Use a Ruby environment compatible with the `github-pages` gem:

```sh
bundle install
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

For a production build, run `bundle exec jekyll build`.
The current legacy Jekyll/Liquid dependencies are incompatible with Ruby 4 without a local compatibility shim; upgrading that toolchain is a separate task.

## Publishing and stale pages

Push changes to the configured GitHub Pages source branch (`master` in this repository).
After the Pages deployment completes, check the homepage and navigation destinations.
GitHub Pages responses can be cached for 10 minutes. If an existing tab shows old content, reload it; use a hard refresh if necessary.

## Theme attribution

Based on [AcademicPages](https://github.com/academicpages/academicpages.github.io), a fork of [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). Original theme copyright and MIT license are retained in `LICENSE` and the theme source files.
