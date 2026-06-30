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
