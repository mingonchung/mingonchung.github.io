# Min-Gon Chung — Personal Academic Website

This repository powers [https://mingonchung.github.io](https://mingonchung.github.io), a Jekyll-based personal/professional website built from the Academic Pages template.

## Repository structure

- `_pages/`: main site pages (home/about, research, publications, teaching, CV).
- `_includes/`, `_layouts/`, `_sass/`: theme templates and styling.
- `_data/`: navigation and author/site metadata.
- `images/`: profile, background, and figure assets.
- `files/`: downloadable files (e.g., CV PDF).
- `assets/`: CSS/JS/fonts used by the site.
- `markdown_generator/`: optional scripts/notebooks for generating publication/talk markdown from TSV data.

## Local development

1. Install dependencies:
   ```bash
   bundle install
   ```
2. Run the site locally:
   ```bash
   bundle exec jekyll serve -l -H localhost
   ```
3. Open <http://localhost:4000>.

## Content updates

- Edit page content in `_pages/`.
- Update sidebar/profile info in `_config.yml` (`author` section).
- Update top navigation in `_data/navigation.yml`.
- Replace files (e.g., CV) in `files/` and update links in page markdown.

## Notes

- Google Analytics is configured centrally in `_config.yml` (`analytics` section).
- This repo intentionally retains most upstream theme assets for compatibility with GitHub Pages.

## Cleanup decisions

To keep the repository lighter and focused on your live site, this repo intentionally removes template-only files that are not part of your current navigation/content workflow:

- `CONTRIBUTING.md` (upstream template contributor guide)
- `_pages/markdown.md` (template markdown demo page)
- `_pages/terms.md` (unused template terms page)
- `_pages/category-archive.html` and `_pages/tag-archive.html` (unused archive pages for blog posts)

