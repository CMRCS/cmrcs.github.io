# Website for the CMRCS group

## Local development

The GitHub Actions workflow builds this site with the official Pages Jekyll
Docker action image. Use the same image locally to avoid host Ruby/Bundler
version mismatches:

```sh
make build
make serve
```

This will rebuild the site, then serves `_site` at `http://localhost:4000`.

Useful overrides:

```sh
PAGES_PORT=5000 scripts/pages-serve
PAGES_DESTINATION=./_site-preview scripts/pages-build
PAGES_JEKYLL_IMAGE=ghcr.io/actions/jekyll-build-pages:v1.0.13 scripts/pages-build
```
