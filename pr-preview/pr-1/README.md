# Website for the CMRCS group

## Development

Use Ruby 3.3.x, then run the full local loop from the repository root:

```sh
export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"
gem install bundler:2.5.23
BUNDLE_PATH=vendor/bundle bundle _2.5.23_ install
BUNDLE_PATH=vendor/bundle bundle _2.5.23_ exec jekyll serve --livereload
BUNDLE_PATH=vendor/bundle bundle _2.5.23_ exec jekyll build
git status --short
```
