# Md Shamim Hussain — research website

This repository serves the static personal site at [shamim-hussain.com](https://shamim-hussain.com).

## Local preview

Run the following from the repository root, then open `http://localhost:8000`.

```sh
python3 -m http.server 8000
```

## Content and assets

- `index.html` contains the homepage and research overview.
- `publications/index.html` contains the complete publication list.
- `css/main.css` contains all styles; the site has no frontend dependencies or build step.
- `img/profile.webp` is the professional portrait.
- `cv.pdf` is the résumé served at the permanent `/cv.pdf` URL. Replace this file when publishing an updated résumé.

## Validation

Before publishing, check the HTML and links locally:

```sh
tidy -qe index.html publications/index.html 404.html
python3 -m http.server 8000
```

## Deployment

GitHub Pages publishes directly from the root of the `master` branch. Develop on a separate branch, review the changes, then merge and push to `master`. The site is published at `https://shamim-hussain.com` using a GitHub Pages custom domain.

