# Project: gherardovarando.uv.es

Personal website for Gherardo Varando, built with Jekyll and the `web-group-theme`.

## Tech Stack
- **Jekyll**: Static site generator (Ruby).
- **Theme**: `gherardovarando/web-group-theme` (loaded via `jekyll-remote-theme`).
- **Plugins**: `jekyll-feed`, `jekyll-seo-tag`, `jekyll-sitemap`, `jekyll-remote-theme`.

## Project Structure
- `_news/`: News items. Files should follow the naming convention `YYYY-MM-DD-title.md`.
- `bibtex/`: Contains `bibtex_gherardovarando.bib` for publications.
- `pdf/`: Academic papers and CV.
- `images/`: Static images.
- `index.md`, `research.md`, `code.md`: Main site pages.

## Workflow & Commands

### Development
Standard Jekyll commands apply:
- Build the site: `bundle exec jekyll build`
- Serve locally: `bundle exec jekyll serve`

Note: The site is configured with `baseurl: "/varando"`, so local testing should account for this path.

### Adding News
1. Create a new file in `_news/` named `YYYY-MM-DD-description.md`.
2. Use the standard layout:
   ```yaml
   ---
   layout: default
   title: "Your News Title"
   ---
   Content goes here.
   ```

### Updating Publications
Update the `bibtex/bibtex_gherardovarando.bib` file. The theme handles the rendering of publications.

## Conventions
- **Naming**: News files MUST start with an ISO date (`YYYY-MM-DD`).
- **Paths**: Always use relative paths or include the `baseurl` when linking internal resources.
