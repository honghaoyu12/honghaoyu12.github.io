# Academic Personal Website

This repository contains a lightweight Jekyll scaffold for an academic personal website that can be deployed to GitHub Pages.

## What Is Included

- a homepage with profile, research interests, and selected work
- standalone pages for publications, projects, talks, teaching, CV, and contact
- Jekyll collections for academic content entries
- a GitHub Actions workflow for GitHub Pages deployment
- simple styling that can be redesigned later without changing the content model

## Project Structure

- `_config.yml`: global site configuration
- `_layouts/`: page layouts
- `_data/navigation.yml`: top navigation items
- `_publications/`: publication entries
- `_projects/`: project entries
- `_talks/`: talk entries
- `_teaching/`: teaching entries
- `assets/css/style.css`: starter styles
- `.github/workflows/pages.yml`: deployment workflow

## Customize First

Update these values before publishing:

1. `title`, `email`, `description`, `url`, and `author` in `_config.yml`
2. homepage text in `index.md`
3. placeholder collection entries in `_publications/`, `_projects/`, `_talks/`, and `_teaching/`
4. links in `cv.md` and `contact.md`

## Run Locally

This scaffold expects a modern Ruby version. If your machine is using an older system Ruby, install Ruby `3.3.x` first with a version manager such as `rbenv`, `asdf`, or `mise`.

Install dependencies:

```bash
bundle install
```

Start the local preview server:

```bash
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

## Deploy To GitHub Pages

1. Create a GitHub repository, ideally named `yourusername.github.io`.
2. Push this project to the repository.
3. In GitHub repository settings, enable GitHub Pages and set the source to GitHub Actions.
4. Push to the default branch to trigger deployment.

## Notes

- This scaffold keeps the design intentionally simple so we can refine the visual design later.
- The site uses standard Jekyll features that work well with GitHub Pages.
