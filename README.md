# Anders Albrechtsen Lab Website

This Jekyll website is based on the [Allan Lab website](https://www.allanlab.org/aboutwebsite.html). Copyright Allan Lab. Code released under the MIT License.

## Local build

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

Before committing changes, verify the production build:

```bash
bundle exec jekyll build
git diff --check
```
