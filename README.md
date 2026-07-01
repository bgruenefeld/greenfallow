# greenfallow labradors

Jekyll/GitHub-Pages site for greenfallow labradors.

## Local development

Install Ruby and Bundler first. On Ubuntu/Debian this is usually:

```bash
sudo apt-get update
sudo apt-get install ruby-full build-essential zlib1g-dev
sudo gem install bundler
```

Then install the project dependencies:

```bash
bundle config set path vendor/bundle
bundle install
```

Start the local Jekyll server:

```bash
bundle exec jekyll serve --livereload
```

The site is available at `http://localhost:4000`.

## Technical privacy notes

The site currently includes the following external services or resources in the source code:

- Google Analytics / Google tag via `googletagmanager.com` in `_includes/custom-head.html`.
- Font Awesome assets are served locally from `assets/fontawesome`.
- Some post and dog pages link to external sites such as DRC, K9Data, Vimeo, Instagram/Facebook and source articles.
- The contact path currently uses a `mailto:` link rather than an embedded contact form.

Impressum and privacy policy should be reviewed editorially and legally after larger technical changes.
